# Comparing `tmp/autora-experimentalist-falsification-1.0.3.tar.gz` & `tmp/autora-experimentalist-falsification-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-falsification-1.0.3.tar", last modified: Mon Jun 19 20:00:39 2023, max compression
+gzip compressed data, was "autora-experimentalist-falsification-1.0.4.tar", last modified: Mon Jul  3 15:24:56 2023, max compression
```

## Comparing `autora-experimentalist-falsification-1.0.3.tar` & `autora-experimentalist-falsification-1.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.360687 autora-experimentalist-falsification-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-19 20:00:39.360687 autora-experimentalist-falsification-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/docs/pooler/
--rw-r--r--   0 runner    (1001) docker     (123)   353052 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/pooler/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/pooler/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    58500 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/pooler/model-vs-data.png
--rw-r--r--   0 runner    (1001) docker     (123)    60582 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/pooler/mse.png
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/pooler/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.360687 autora-experimentalist-falsification-1.0.3/docs/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)   350086 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/sampler/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/sampler/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    58500 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/sampler/model-vs-data.png
--rw-r--r--   0 runner    (1001) docker     (123)    60582 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/sampler/mse.png
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/docs/sampler/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.360687 autora-experimentalist-falsification-1.0.3/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 20:00:39.360687 autora-experimentalist-falsification-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/src/autora/experimentalist/pooler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.360687 autora-experimentalist-falsification-1.0.3/src/autora/experimentalist/pooler/falsification/
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/src/autora/experimentalist/pooler/falsification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.356687 autora-experimentalist-falsification-1.0.3/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.360687 autora-experimentalist-falsification-1.0.3/src/autora/experimentalist/sampler/falsification/
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/src/autora/experimentalist/sampler/falsification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.360687 autora-experimentalist-falsification-1.0.3/src/autora_experimentalist_falsification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-19 20:00:39.000000 autora-experimentalist-falsification-1.0.3/src/autora_experimentalist_falsification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-19 20:00:39.000000 autora-experimentalist-falsification-1.0.3/src/autora_experimentalist_falsification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:00:39.000000 autora-experimentalist-falsification-1.0.3/src/autora_experimentalist_falsification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 20:00:39.000000 autora-experimentalist-falsification-1.0.3/src/autora_experimentalist_falsification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 20:00:39.000000 autora-experimentalist-falsification-1.0.3/src/autora_experimentalist_falsification.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:39.360687 autora-experimentalist-falsification-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/tests/test_exp_falsification_pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-19 20:00:29.000000 autora-experimentalist-falsification-1.0.3/tests/test_exp_falsification_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.434670 autora-experimentalist-falsification-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-03 15:24:56.434670 autora-experimentalist-falsification-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/docs/pooler/
+-rw-r--r--   0 runner    (1001) docker     (123)   351750 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/pooler/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/pooler/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    58500 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/pooler/model-vs-data.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60582 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/pooler/mse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/pooler/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.434670 autora-experimentalist-falsification-1.0.4/docs/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)   348550 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/sampler/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/sampler/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    58500 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/sampler/model-vs-data.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60582 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/sampler/mse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/docs/sampler/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.434670 autora-experimentalist-falsification-1.0.4/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:24:56.434670 autora-experimentalist-falsification-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/src/autora/experimentalist/pooler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.434670 autora-experimentalist-falsification-1.0.4/src/autora/experimentalist/pooler/falsification/
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/src/autora/experimentalist/pooler/falsification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.430670 autora-experimentalist-falsification-1.0.4/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.434670 autora-experimentalist-falsification-1.0.4/src/autora/experimentalist/sampler/falsification/
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/src/autora/experimentalist/sampler/falsification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.434670 autora-experimentalist-falsification-1.0.4/src/autora_experimentalist_falsification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-03 15:24:56.000000 autora-experimentalist-falsification-1.0.4/src/autora_experimentalist_falsification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-03 15:24:56.000000 autora-experimentalist-falsification-1.0.4/src/autora_experimentalist_falsification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:24:56.000000 autora-experimentalist-falsification-1.0.4/src/autora_experimentalist_falsification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 15:24:56.000000 autora-experimentalist-falsification-1.0.4/src/autora_experimentalist_falsification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 15:24:56.000000 autora-experimentalist-falsification-1.0.4/src/autora_experimentalist_falsification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:56.434670 autora-experimentalist-falsification-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/tests/test_exp_falsification_pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-07-03 15:24:44.000000 autora-experimentalist-falsification-1.0.4/tests/test_exp_falsification_sampler.py
```

### Comparing `autora-experimentalist-falsification-1.0.3/.github/workflows/python-publish.yml` & `autora-experimentalist-falsification-1.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/.github/workflows/test-pytest.yml` & `autora-experimentalist-falsification-1.0.4/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/.gitignore` & `autora-experimentalist-falsification-1.0.4/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -63,7 +63,10 @@
 
 # Material for MkDocs
 site/
 docs/reference/
 
 # Jupyter Notebook load data
 .ipynb_checkpoints
+
+# IDE Files
+/.idea/
```

### Comparing `autora-experimentalist-falsification-1.0.3/.pre-commit-config.yaml` & `autora-experimentalist-falsification-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/PKG-INFO` & `autora-experimentalist-falsification-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-falsification
-Version: 1.0.3
+Version: 1.0.4
 Summary: AutoRA Falsification Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-falsification
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
```

### Comparing `autora-experimentalist-falsification-1.0.3/README.md` & `autora-experimentalist-falsification-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/docs/pooler/Basic Usage.ipynb` & `autora-experimentalist-falsification-1.0.4/docs/pooler/Basic Usage.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99165469348659%*

 * *Differences: {"'cells'": "{0: {'metadata': {delete: ['pycharm']}}, 2: {'metadata': {delete: ['pycharm']}}, 3: "*

 * *            "{'metadata': {delete: ['pycharm']}}, 4: {'metadata': {delete: ['pycharm']}}, 5: "*

 * *            "{'metadata': {delete: ['pycharm']}, 'source': {insert: [(0, '## Example 1: Sampling "*

 * *            "From A Sine Function\\n')], delete: [0]}}, 6: {'metadata': {delete: ['pycharm']}}, 7: "*

 * *            "{'metadata': {delete: ['pycharm']}}, 8: {'metadata': {delete: ['pycharm']}}, 9: "*

 * *            "{'metadata […]*

```diff
@@ -1,17 +1,14 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "# Basic Usage\n",
                 "The falsification pooler identifies experiment conditions under which the loss $\\hat{\\mathcal{L}}(M,X,Y,X')$ of the best candidate model is predicted to be the highest. This loss is approximated with a multi-layer perceptron, which is trained to predict the loss of a candidate model, $M$, given experiment conditions $X$  and dependent measures $Y$ that have already been probed.\n",
                 "\n",
                 "We begin with importing the relevant packages."
             ]
@@ -26,106 +23,85 @@
                 "# !pip install \"autora[experimentalist-falsification]\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from sklearn.linear_model import LinearRegression\n",
                 "from autora.variable import DV, IV, ValueType, VariableCollection\n",
                 "from autora.experimentalist.pooler.falsification import falsification_pool"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "In order to reproduce our results, we also import torch and set the seed."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import torch\n",
                 "torch.manual_seed(180)\n",
                 "np.random.seed(180)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
-                "## Example 1: Sampling fom a Sinus Function\n",
+                "## Example 1: Sampling From A Sine Function\n",
                 "\n",
                 "In this example, we will consider a dataset resembling the sine function. We will then fit a linear model to the data and use the falsification pooler to identify experiment conditions under which the model is predicted to perform the worst.\n",
                 "\n",
                 "First, we define the experiment conditions $X$ and the observations $Y$. We consider a domain of $X \\in [0, 2\\pi]$, and sample 100 data points from this domain."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "X = np.linspace(0, 2 * np.pi, 100)\n",
                 "Y = np.sin(X)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Next, we need to define metadata object, so the falsification pooler knows what data it is supposed to generate. We can do this by defining the independent variable $x$, which underlies experimental conditions $X$, and the dependent variable $y$, which underlies the observations $Y$. We specify that $x$ is a continuous variable with a range of $[0, 2\\pi]$, and $y$ is a real-valued variable."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "# Specify independent variable\n",
                 "iv = IV(\n",
                 "    name=\"x\",\n",
                 "    value_range=(0, 2 * np.pi),\n",
@@ -143,31 +119,25 @@
                 "    dependent_variables=[dv],\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Next, we can specify the model that we would like to fit to the data. In this case, we will use a linear model."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LinearRegression()</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LinearRegression</label><div class=\"sk-toggleable__content\"><pre>LinearRegression()</pre></div></div></div></div></div>"
                         ],
@@ -184,31 +154,25 @@
                 "model = LinearRegression()\n",
                 "model.fit(X.reshape(-1, 1), Y)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Finally, we can generate novel experimental conditions $X'$ from the falsification pooler. We will generate 10 novel experimental conditions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "image/png": "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pUuXuOWWW8jJyWHatGn4+/uzZMkSbrvtNn744Qduv/12g/3feOMN1Go1Tz/9NOnp6bz11luMHTuW3bt3V/n+SkRGRjJhwgQWLFjAc889V+Uxf+2113jxxRcZPXo09913HykpKXzwwQf06tWLv/76Cx8fH1544QXS09M5e/Ys7733HgAeHh6oVCq6d+/O1q1b9c/3zz//kJ6ejlqtZvv27QwbNgyA33//nXbt2ukLe405N0sbNWoUMTExvP766yiKUuF7+eOPP4iPj6djx46sWLECV1dXo46XsCGKEFZs0aJFCqBs2LBBSUlJUc6cOaN88803ir+/v+Lq6qqcPXtWURRFmThxogIozz33nMHjf//9dwVQvvrqK4Pta9asMdh++fJlxcnJSRk2bJii1Wr1+z3//PMKoEycOFG/bdOmTQqgbNq0SVEURSksLFQiIyOV8PBw5erVqwavU/q5pk6dqlT2KwcoM2fO1P88cuRIxcnJSUlKStJvO3/+vOLp6an06tWr3PEZMGCAwWs9+eSTikajUa5du1bh65Vo27atEhQUpFy5ckW/7e+//1bUarUyYcKEcu/5+++/r/L5Su9b0S05OVnJzc1VioqKDB6TnJysODs7Ky+//LLBNkBZtGiRoiiKcvXqVQVQ3n777Spfv3fv3krv3r0NtgHK1KlTK4yzpp9jTk5OuddcunSpAihbt27Vb3v77bf177ms8PBwg3PqiSeeUADl999/12/LzMxUIiMjlYiICP3xKok5Li5OycvL0+87b948BVD2799f4TEpUXK+/PHHH0pSUpLi4OCgTJs2TX9/7969lRYtWuh/PnnypKLRaJTXXnvN4Hn279+vODg4GGwfNmyYEh4eXu413377bUWj0SgZGRmKoijK+++/r4SHhyudO3dWnn32WUVRFKWoqEjx8fFRnnzySf3jjD03Z86cqQDKPffcU+61J06cqLi7uyuKoijbtm1TvLy8lGHDhim5ublVHidhu6T7SdiEAQMGEBgYSFhYGHfffTceHh4sW7aMhg0bGuz38MMPG/z8/fff4+3tzcCBA0lNTdXfOnTogIeHB5s2bQJ03wrz8/N57LHHDLqFjCl6/Ouvv0hOTuaJJ54oV7dR+rmMVVRUxLp16xg5ciRNmjTRbw8NDWXMmDFs27aNjIwMg8c88MADBq/Vs2dPioqKOHXqVKWv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G8eWLVsAXfJ1xx13MHz4cBISErjvvvt47rnnjDoOwcHBxMfHs2TJEgBycnL49ttvmTJlisF+ISEhFBYWsmzZsps+9qVlZ2cTHx+Pr68vf/zxB99//z0bNmzg0UcfBeDpp5/Wt4aUtPqUVdWxA1iyZAnu7u7s3r2bt956i5dffpn169fr7x81ahSXL19m9erV7N27l/bt29O/f3/S0tKqjL1Dhw5EREToX/v06dNs3bqV8ePH1+g9gnHnUnXngbBRVnYtlMn3aisqSv/fNTHdSPJvRPyxnURfOavbGB1tocCEsa4XFNH8pbUWee1DL8fj5lTzXz9FUdi4cSNr167lscce0293d3fns88+08/B8+WXX6LVavnss8/0rQOLFi3Cx8eHzZs3M2jQIObOncuMGTO44447APj4449Zu7by45GYmMh3333H+vXrGTBgAABNmjTR3+/n5wdAUFAQPj4+gK5l5/XXX2fDhg1069ZN/5ht27bxySef0Lt3b+bPn09UVBTvvvsuAE2bNmX//v28+eabRh2TKVOm8NRTT/HCCy/www8/EBUVRdu2bQ326dq1K88//zxjxozhoYceonPnzvTr148JEyYQHBxssO8tt9xSbrbp0q0SpX399dfk5uby+eef67u7PvzwQ4YPH86bb75JcHCw/liEhIRU+BwajabCY1eidevWzJw5E4CYmBg+/PBDNm7cyMCBA9m2bRt79uzh8uXL+m6td955h+XLl/PDDz/wwAMPVHvsFi5cyLhx41i8eDFDhw4lMDCwxu+xunPJmPNA2KhS18IK1fG1UJKa2oqNhfh42LCBL9oPY3tEW0IzU4m+dgEGDICYGEtHKOzIypUr8fDwoKCgAK1Wy5gxYwy6IVq1amUwqeDff//N8ePHy9XD5ObmkpSURHp6OhcuXKBLly76+xwcHOjYsWOlLRkJCQloNJoaXYCOHz9OTk4OAwcONNien59Pu3btAF0hbek4AP2FzxjDhg3jwQcfZOvWrSxcuLBcK02J1157jenTp/Pbb7+xe/duPv74Y15//XW2bt1Kq1at9Pt9++23xMXFGfXahw8fpk2bNgb1O927d0er1XL06NFyCVNttG7d2uDn0NBQfXHz33//TVZWFv7+/gb7XL9+XV/LU5Vx48bx3HPPceLECRYvXsz7779fbp/q3qOLi0u155Ix54GwUaWu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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
@@ -249,18 +213,15 @@
                 "    )"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Before we examine the novel conditions, let's have a look at the three plots generated by the falsification pooler, going from last to first.\n",
                 "\n",
                 "- **Model Prediction vs. Data**. The model trained on the data is shown in red, and the model prediction is shown in blue. The model prediction is a straight line, which is a poor fit to the data. This is expected, since the data is generated from a sine function, which is not linear. <br> <br>\n",
                 "\n",
                 "- **Loss of the Falsification Network**. The plot shows the learning curve for the falsification network that is trained to predict the error of the (linear) model as a function of experimental conditions. The error (loss) of this network decreases as a function of the number of training epochs. <br> <br>\n",
@@ -272,18 +233,15 @@
                 "Before examining the new conditions, we need to convert them to a numpy array."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[0.        ]\n",
@@ -303,31 +261,25 @@
                 "new_conditions = np.array(list(new_conditions))\n",
                 "print(new_conditions)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Note that the new conditions are all at the limits of the domain $\\{0, 2\\pi\\}$, as well as around the peaks of the sinusoid, which is expected since the model is a poor fit to the data at those points. We can also plot the new conditions on top of the data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<matplotlib.legend.Legend at 0x143766310>"
                         ]
@@ -357,62 +309,50 @@
                 "ax.set_ylabel(\"Y\")\n",
                 "ax.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
-                "## Example 2: Sampling from a Gaussian Mixture Model\n",
+                "## Example 2: Sampling From A Gaussian Mixture Model\n",
                 "\n",
                 "In this example, we will consider a dataset sampled from a Gaussian mixture model. We will fit a Gaussian mixture model to the data and use the falsification pooler to identify experiment conditions under which the model is predicted to perform the worst.\n",
                 "\n",
                 "First, we define the experimental conditions $X$ and the observations $Y$, and sample 100 data points. The dependent variable is a categorical variable with 2 categories."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from sklearn.datasets import make_blobs\n",
                 "X, Y = make_blobs(n_samples=100, n_features=1, centers=2, random_state=0)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Next, we need to define metadata object, so the falsification pooler knows what data it is supposed to generate. We can do this by defining the independent variable $x$ underlying the experimental conditions $X$ and the dependent variable $y$ underlying the observations $Y$ as \"VariableCollection\" objects. We specify that $X$ is a continuous variable with a range of $[-1, 6]$, and $Y$ is a categorical variable."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "# Specify independent variable\n",
                 "iv = IV(\n",
                 "    name=\"X\",\n",
                 "    value_range=(-1, 6),\n",
@@ -430,31 +370,25 @@
                 "    dependent_variables=[dv],\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Next, we can specify the model that we would like to fit to the data. In this case, we will use a Gaussian mixture model with 2 components."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<matplotlib.legend.Legend at 0x143aaf070>"
                         ]
@@ -488,31 +422,25 @@
                 "ax.set_ylabel(\"Y\")\n",
                 "ax.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "In this case, the model appears to predict most of the data points quite well but fails to predict data points around $x=3$. Let's see if the falsification pooler can identify this region of the domain."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
@@ -552,31 +480,25 @@
                 "        plot=True,\n",
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "As shown in the \"Prediction of Falsification Network\" plot, the model is predicted to perform the worst around $x=3$. Let's have a look at the new conditions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[2.53794861]\n",
@@ -596,31 +518,25 @@
                 "new_conditions = np.array(list(new_conditions))\n",
                 "print(new_conditions)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Indeed, the new conditions mostly located around $x=3$, reflecting a poor fit of the model for those conditions. Finally, we can plot the new conditions on top of the data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<matplotlib.legend.Legend at 0x1436958e0>"
                         ]
```

### Comparing `autora-experimentalist-falsification-1.0.3/docs/pooler/index.md` & `autora-experimentalist-falsification-1.0.4/docs/pooler/index.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/docs/pooler/model-vs-data.png` & `autora-experimentalist-falsification-1.0.4/docs/pooler/model-vs-data.png`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/docs/pooler/mse.png` & `autora-experimentalist-falsification-1.0.4/docs/pooler/mse.png`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/docs/sampler/Basic Usage.ipynb` & `autora-experimentalist-falsification-1.0.4/docs/sampler/Basic Usage.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991671772875817%*

 * *Differences: {"'cells'": "{0: {'metadata': {delete: ['pycharm']}}, 2: {'metadata': {delete: ['pycharm']}}, 3: "*

 * *            "{'metadata': {delete: ['pycharm']}}, 4: {'metadata': {delete: ['pycharm']}}, 5: "*

 * *            "{'metadata': {delete: ['pycharm']}, 'source': {insert: [(0, '## Example 1: Sampling "*

 * *            "From A Sine Function\\n')], delete: [0]}}, 6: {'metadata': {delete: ['pycharm']}}, 7: "*

 * *            "{'metadata': {delete: ['pycharm']}}, 8: {'metadata': {delete: ['pycharm']}}, 9: "*

 * *            "{'metadata […]*

```diff
@@ -1,17 +1,14 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "# Basic Usage\n",
                 "The falsification sampler identifies experiment conditions under which the loss $\\hat{\\mathcal{L}}(M,X,Y,\\vec{x})$ of the best candidate model is predicted to be the highest. This loss is approximated with a multi-layer perceptron, which is trained to predict the loss of a candidate model, $M$, given experiment conditions $X$  and dependent measures $Y$ that have already been probed.\n",
                 "\n",
                 "We begin with importing the relevant packages."
             ]
@@ -26,106 +23,85 @@
                 "# !pip install \"autora[experimentalist-falsification]\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from sklearn.linear_model import LinearRegression\n",
                 "from autora.variable import DV, IV, ValueType, VariableCollection\n",
                 "from autora.experimentalist.sampler.falsification import falsification_sample, falsification_score_sample"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "In order to reproduce our results, we also import torch and set the seed."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "import torch\n",
                 "torch.manual_seed(180)\n",
                 "np.random.seed(180)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
-                "## Example 1: Sampling fom a Sinus Function\n",
+                "## Example 1: Sampling From A Sine Function\n",
                 "\n",
                 "In this example, we will consider a dataset resembling the sine function. We will then fit a linear model to the data and use the falsification sampler to identify experiment conditions under which the model is predicted to perform the worst.\n",
                 "\n",
                 "First, we define the experiment conditions $X$ and the observations $Y$. We consider a domain of $X \\in [0, 2\\pi]$, and sample 100 data points from this domain."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "X = np.linspace(0, 2 * np.pi, 100)\n",
                 "Y = np.sin(X)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Next, we need to define metadata object, so the falsification sampler knows what data it is supposed to generate. We can do this by defining the independent variable $x$, which underlies experimental conditions $X$, and the dependent variable $y$, which underlies the observations $Y$. We specify that $x$ is a continuous variable with a range of $[0, 2\\pi]$, and $y$ is a real-valued variable."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "# Specify independent variable\n",
                 "iv = IV(\n",
                 "    name=\"x\",\n",
                 "    value_range=(0, 2 * np.pi),\n",
@@ -143,31 +119,25 @@
                 "    dependent_variables=[dv],\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Next, we can specify the model that we would like to fit to the data. In this case, we will use a linear model."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>LinearRegression()</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">LinearRegression</label><div class=\"sk-toggleable__content\"><pre>LinearRegression()</pre></div></div></div></div></div>"
                         ],
@@ -184,31 +154,25 @@
                 "model = LinearRegression()\n",
                 "model.fit(X.reshape(-1, 1), Y)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Finally, we can generate novel experimental conditions $X'$ from the falsification sampler. We will select 5 novel experimental conditions from a candidate set of 14 experiment conditions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "image/png": "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pUuXuOWWW8jJyWHatGn4+/uzZMkSbrvtNn744Qduv/12g/3feOMN1Go1Tz/9NOnp6bz11luMHTuW3bt3V/n+SkRGRjJhwgQWLFjAc889V+Uxf+2113jxxRcZPXo09913HykpKXzwwQf06tWLv/76Cx8fH1544QXS09M5e/Ys7733HgAeHh6oVCq6d+/O1q1b9c/3zz//kJ6ejlqtZvv27QwbNgyA33//nXbt2ukLe405N0sbNWoUMTExvP766yiKUuF7+eOPP4iPj6djx46sWLECV1dXo46XsCGKEFZs0aJFCqBs2LBBSUlJUc6cOaN88803ir+/v+Lq6qqcPXtWURRFmThxogIozz33nMHjf//9dwVQvvrqK4Pta9asMdh++fJlxcnJSRk2bJii1Wr1+z3//PMKoEycOFG/bdOmTQqgbNq0SVEURSksLFQiIyOV8PBw5erVqwavU/q5pk6dqlT2KwcoM2fO1P88cuRIxcnJSUlKStJvO3/+vOLp6an06tWr3PEZMGCAwWs9+eSTikajUa5du1bh65Vo27atEhQUpFy5ckW/7e+//1bUarUyYcKEcu/5+++/r/L5Su9b0S05OVnJzc1VioqKDB6TnJysODs7Ky+//LLBNkBZtGiRoiiKcvXqVQVQ3n777Spfv3fv3krv3r0NtgHK1KlTK4yzpp9jTk5OuddcunSpAihbt27Vb3v77bf177ms8PBwg3PqiSeeUADl999/12/LzMxUIiMjlYiICP3xKok5Li5OycvL0+87b948BVD2799f4TEpUXK+/PHHH0pSUpLi4OCgTJs2TX9/7969lRYtWuh/PnnypKLRaJTXXnvN4Hn279+vODg4GGwfNmyYEh4eXu413377bUWj0SgZGRmKoijK+++/r4SHhyudO3dWnn32WUVRFKWoqEjx8fFRnnzySf3jjD03Z86cqQDKPffcU+61J06cqLi7uyuKoijbtm1TvLy8lGHDhim5ublVHidhu6T7SdiEAQMGEBgYSFhYGHfffTceHh4sW7aMhg0bGuz38MMPG/z8/fff4+3tzcCBA0lNTdXfOnTogIeHB5s2bQJ03wrz8/N57LHHDLqFjCl6/Ouvv0hOTuaJJ54oV7dR+rmMVVRUxLp16xg5ciRNmjTRbw8NDWXMmDFs27aNjIwMg8c88MADBq/Vs2dPioqKOHXqVKWv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G8eWLVsAXfJ1xx13MHz4cBISErjvvvt47rnnjDoOwcHBxMfHs2TJEgBycnL49ttvmTJlisF+ISEhFBYWsmzZsps+9qVlZ2cTHx+Pr68vf/zxB99//z0bNmzg0UcfBeDpp5/Wt4aUtPqUVdWxA1iyZAnu7u7s3r2bt956i5dffpn169fr7x81ahSXL19m9erV7N27l/bt29O/f3/S0tKqjL1Dhw5EREToX/v06dNs3bqV8ePH1+g9gnHnUnXngbBRVnYtlMn3aisqSv/fNTHdSPJvRPyxnURfOavbGB1tocCEsa4XFNH8pbUWee1DL8fj5lTzXz9FUdi4cSNr167lscce0293d3fns88+08/B8+WXX6LVavnss8/0rQOLFi3Cx8eHzZs3M2jQIObOncuMGTO44447APj4449Zu7by45GYmMh3333H+vXrGTBgAABNmjTR3+/n5wdAUFAQPj4+gK5l5/XXX2fDhg1069ZN/5ht27bxySef0Lt3b+bPn09UVBTvvvsuAE2bNmX//v28+eabRh2TKVOm8NRTT/HCCy/www8/EBUVRdu2bQ326dq1K88//zxjxozhoYceonPnzvTr148JEyYQHBxssO8tt9xSbrbp0q0SpX399dfk5uby+eef67u7PvzwQ4YPH86bb75JcHCw/liEhIRU+BwajabCY1eidevWzJw5E4CYmBg+/PBDNm7cyMCBA9m2bRt79uzh8uXL+m6td955h+XLl/PDDz/wwAMPVHvsFi5cyLhx41i8eDFDhw4lMDCwxu+xunPJmPNA2KhS18IK1fG1UJKa2oqNhfh42LCBL9oPY3tEW0IzU4m+dgEGDICYGEtHKOzIypUr8fDwoKCgAK1Wy5gxYwy6IVq1amUwqeDff//N8ePHy9XD5ObmkpSURHp6OhcuXKBLly76+xwcHOjYsWOlLRkJCQloNJoaXYCOHz9OTk4OAwcONNien59Pu3btAF0hbek4AP2FzxjDhg3jwQcfZOvWrSxcuLBcK02J1157jenTp/Pbb7+xe/duPv74Y15//XW2bt1Kq1at9Pt9++23xMXFGfXahw8fpk2bNgb1O927d0er1XL06NFyCVNttG7d2uDn0NBQfXHz33//TVZWFv7+/gb7XL9+XV/LU5Vx48bx3HPPceLECRYvXsz7779fbp/q3qOLi0u155Ix54GwUaWu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",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
@@ -252,18 +216,15 @@
                 "    )"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Before we examine the novel conditions, let's have a look at the three plots generated by the falsification sampler, going from last to first.\n",
                 "\n",
                 "- **Model Prediction vs. Data**. The model trained on the data is shown in red, and the model prediction is shown in blue. The model prediction is a straight line, which is a poor fit to the data. This is expected, since the data is generated from a sine function, which is not linear. <br> <br>\n",
                 "\n",
                 "- **Loss of the Falsification Network**. The plot shows the learning curve for the falsification network that is trained to predict the error of the (linear) model as a function of experimental conditions. The error (loss) of this network decreases as a function of the number of training epochs. <br> <br>\n",
@@ -275,18 +236,15 @@
                 "Before examining the selected new conditions, we need to convert them to a numpy array."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[0. ]\n",
@@ -301,31 +259,25 @@
                 "new_conditions = np.array(list(new_conditions))\n",
                 "print(new_conditions)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Note that the new conditions are all at the limits of the domain $\\{0, 2\\pi\\}$, as well as around the peaks of the sinusoid, which is expected since the model is a poor fit to the data at those points. We can also plot the new conditions on top of the data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<matplotlib.legend.Legend at 0x143372ca0>"
                         ]
@@ -355,42 +307,33 @@
                 "ax.set_ylabel(\"Y\")\n",
                 "ax.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": []
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "We can also obtain \"falsification\" scores for the sampled experiment conditions using ``falsification_score_sample''. The scores are z-scored with respect to all conditions from the candidate set. In the following example, we sample 5 conditions and return their falsification scores."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[6.5]\n",
@@ -415,62 +358,50 @@
                 "print(new_conditions)\n",
                 "print(scores)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
-                "## Example 2: Sampling from a Gaussian Mixture Model\n",
+                "## Example 2: Sampling From A Gaussian Mixture Model\n",
                 "\n",
                 "In this example, we will consider a dataset sampled from a Gaussian mixture model. We will fit a Gaussian mixture model to the data and use the falsification sampler to identify experiment conditions under which the model is predicted to perform the worst.\n",
                 "\n",
                 "First, we define the experimental conditions $X$ and the observations $Y$, and sample 100 data points. The dependent variable is a categorical variable with 2 categories."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from sklearn.datasets import make_blobs\n",
                 "X, Y = make_blobs(n_samples=100, n_features=1, centers=2, random_state=0)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Next, we need to define metadata object, so the falsification sampler knows what data it is supposed to generate. We can do this by defining the independent variable $x$ underlying the experimental conditions $X$ and the dependent variable $y$ underlying the observations $Y$ as \"VariableCollection\" objects. We specify that $X$ is a continuous variable with a range of $[-1, 6]$, and $Y$ is a categorical variable."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "# Specify independent variable\n",
                 "iv = IV(\n",
                 "    name=\"X\",\n",
                 "    value_range=(-1, 6),\n",
@@ -488,31 +419,25 @@
                 "    dependent_variables=[dv],\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Next, we can specify the model that we would like to fit to the data. In this case, we will use a Gaussian mixture model with 2 components."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<matplotlib.legend.Legend at 0x1434796a0>"
                         ]
@@ -546,57 +471,45 @@
                 "ax.set_ylabel(\"Y\")\n",
                 "ax.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "In this case, the model appears to predict most of the data points quite well but fails to predict data points around $x=3$. Let's see if the falsification sampler can identify this region of the domain. We will select samples from a candidate set of 71 experiment conditions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [],
             "source": [
                 "X_prime = np.linspace(-1, 6, 71)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "and call the falsification sampler."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "image/png": "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m+mxTC1YsAAxMTHQarWoX78+vvzyS7PHJUnC4sWLMWDAAHh5eaFevXr46aefbJ6bjh074oUXXsDo0aORnZ2NuXPnIikpCYsXL3boHBM5ExMVogokf2kNHz4c6enpOHjwIF5//XUsXrwYoaGhynrLli2DRqPBvn37MHfuXHz00UdmXybPP/88du/ejRUrVuDvv//GwIED0bNnT7Mv2pycHLz77rtYvHgxjhw5gpCQEIsxLVu2DNWrV8e+ffvwwgsv4Nlnn8XAgQPx4IMP4sCBA+jRoweGDx+OnJwcAMYWi65du6J58+b4448/sH79ely5cgWDBg0qsV9vb2/s3bsX7733HmbOnImNGzcCAPbv3w8ASExMRGpqqnI/KysLvXv3xubNm3Hw4EH07NkTffv2xblz5+w6vwaDAStWrMDQoUNRo0aNEo/7+PhAozE2HI8aNQp//PEHfvrpJ+zevRtCCPTu3RsFBQVm5/CDDz7Al19+ie3bt+PcuXOYPHmy8viHH36IpUuXYsmSJdi5cyfS0tKwevVqq/GtWrUKtWrVwsyZM5GammqW9JhavXo1xo8fjxdffBGHDx/G008/jdGjR2PLli1m682YMQODBg3C33//jd69e2Po0KFIS0uzeY7efvttaDQaDBs2DP/+978xb9481KxZ0+Y2RC7FiRdEJKryRo4cKdRqtfD29ja7vf3228o6eXl5olmzZmLQoEGiYcOG4sknnzTbR6dOnURcXJwwGAzKsldeeUXExcUJIYQ4e/asUKvV4uLFi2bbdevWTUydOlUIIURiYqIAIJKSkkrE169fP7NjtW/fXrmv0+mEt7e3GD58uLIsNTVVABC7d+8WQgjx5ptvih49epjt9/z58wKAOH78uMX9CiFEq1atxCuvvKLcByBWr15t4Syaa9SokZg3b55yPzIyUnz88ccW171y5YoAID766COb+0xOThYAxK5du5Rl169fF56enuLbb78VQhSdQ9Mr586fP1+EhoYq98PDw8V7772n3C8oKBC1atUqcY5NrzJsKf7ExETh7++v3H/wwQdLvC4GDhwoevfurdwHIF577TXlflZWlgAg1q1bZ/O5CyHE+vXrBQDRq1evUtclcjWsUSG6Q126dMGCBQvMlpnWKWi1Wnz99ddo0qQJIiMj8fHHH5fYxwMPPKB0CwBA27Zt8eGHH0Kv1+PQoUPQ6/WIjY012yYvLw9BQUFmx2nSpEmp8Zquo1arERQUhMaNGyvL5Jaeq1evAgD++usvbNmyRelCMZWSkqLEVfzY4eHhyj6sycrKwvTp0/Hzzz8jNTUVOp0Ot2/ftrtFRdhZKHvs2DFoNBq0adNGWRYUFIT69evj2LFjyjIvLy/ExMRYfA7p6elITU0124dGo0HLli3vuGD32LFjeOqpp8yWtWvXDnPnzjVbZnqOvb294efnV+o5BoD//ve/8PLywqFDh5Cenn5P1C7R3YOJCtEd8vb2Rt26dW2u8/vvvwMA0tLSkJaWBm9vb7v3n5WVBbVajT///BNqtdrsMdPkwdPT0yzZscbNzc3sviRJZsvkfRgMBuX4ffv2xbvvvltiX+Hh4Tb3K+/DmsmTJ2Pjxo344IMPULduXXh6euKRRx5Bfn5+qc8DAIKDgxEQEIB//vnHrvVLY+k53GkSUp7Kco5XrlyJtWvXYvfu3Rg8eDAmTpyIJUuWVGSYROWKNSpEFSwlJQUTJ07EokWL0KZNG4wcObLEl8vevXvN7u/Zswf16tWDWq1G8+bNodfrcfXqVdStW9fsFhYWVuHx33///Thy5AiioqJKHN+RhMvNzQ16vd5s2a5duzBq1CgMGDAAjRs3RlhYGM6cOWP3PlUqFR577DF8/fXXuHTpUonHs7KyoNPpEBcXB51OZ3aeb9y4gePHj6Nhw4Z2Hcvf3x/h4eFm+9DpdPjzzz9tbqfVaks87+Li4uKwa9cus2W7du2yOzZrrly5grFjx+Ktt95C06ZNsXTpUnzxxRcliqWJXBkTFaI7lJeXh8uXL5vd5BExer0ew4YNQ0JCAkaPHo3ExET8/fff+PDDD832ce7cOUyaNAnHjx/H8uXLMW/ePIwfPx4AEBsbi6FDh2LEiBFYtWoVTp8+jX379mHWrFn4+eefK/z5jR07FmlpaRg8eDD279+PlJQUbNiwAaNHjy71C9hUVFQUNm/ejMuXL+PmzZsAgHr16mHVqlVISkrCX3/9hSFDhpTaQlDc22+/jYiICLRp0wZffPEFjh49ihMnTmDJkiVo3rw5srKyUK9ePfTr1w9PPvkkdu7cib/++gvDhg1DzZo10a9fP7uPNX78eMyePRtr1qzBP//8g+eeew63bt0q9Xlv374dFy9eNBspZeqll17C0qVLsWDBApw4cQIfffQRVq1aZVbIWxZPPfUU4uLilFFIrVu3xksvvYSnnnoK6enpd7RvosrCRIXoDq1fvx7h4eFmt/bt2wMwfomePXsWCxcuBGDsKvn888/x2muv4a+//lL2MWLECNy+fRutW7fG2LFjMX78eLOahcTERIwYMQIvvvgi6tevj/79+2P//v2oXbt2hT+/GjVqYNeuXdDr9ejRowcaN26MCRMmICAgACqV/R8hH374ITZu3IiIiAg0b94cAPDRRx8hMDAQDz74IPr27YuEhATcf//9DsVXrVo17NmzB8OGDcNbb72F5s2bo0OHDli+fDnef/99pR4jMTERLVq0wEMPPYS2bdtCCIFffvmlRHeKLS+++CKGDx+OkSNHom3btvD19cWAAQNsbjNz5kycOXMGMTExCA4OtrhO//79MXfuXHzwwQdo1KgRFi5ciMTERHTu3Nnu2Ir74osvsGnTJiQmJpr9nWbMmIGAgABMnDixzPsmqkyScKUOWKJ7UOfOndGsWTOXniaeiMhZ2KJCRERELouJChEREbksdv0QERGRy2KLChEREbksJipERETkspioEBERkctiokJEREQui4kKERERuSwmKkREROSymKgQERGRy2KiQkRERC6LiQoRERG5rP8HRpHaGsv7XPgAAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
@@ -637,31 +550,25 @@
                 "        plot=True,\n",
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "As shown in the \"Prediction of Falsification Network\" plot, the model is predicted to perform the worst around $x=3$. Let's have a look at the selected new conditions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[2.9]\n",
@@ -681,31 +588,25 @@
                 "new_conditions = np.array(list(new_conditions))\n",
                 "print(new_conditions)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": false
             },
             "source": [
                 "Indeed, the new conditions mostly located around $x=3$, reflecting a poor fit of the model for those conditions. Finally, we can plot the new conditions on top of the data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {
-                "collapsed": false,
-                "pycharm": {
-                    "name": "#%%\n"
-                }
+                "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<matplotlib.legend.Legend at 0x145ed8d00>"
                         ]
```

### Comparing `autora-experimentalist-falsification-1.0.3/docs/sampler/index.md` & `autora-experimentalist-falsification-1.0.4/docs/sampler/index.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/docs/sampler/model-vs-data.png` & `autora-experimentalist-falsification-1.0.4/docs/sampler/model-vs-data.png`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/docs/sampler/mse.png` & `autora-experimentalist-falsification-1.0.4/docs/sampler/mse.png`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/mkdocs/base.yml` & `autora-experimentalist-falsification-1.0.4/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/mkdocs.yml` & `autora-experimentalist-falsification-1.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/pyproject.toml` & `autora-experimentalist-falsification-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 authors = [{ name = "Sebastian Musslick", email = "sebastian@musslick.de" }]
 dynamic = ["version"]
 readme = "README.md"
 license = { text = "MIT License" }
 
 # ADD NEW DEPENDENCIES HERE
 dependencies = [
-    "autora-core",
+    "autora-core>=3.1.0",
     "torch"
 ]
 
 [project.optional-dependencies]
 dev = [
     "autora-core[dev]"
 ]
```

### Comparing `autora-experimentalist-falsification-1.0.3/src/autora/experimentalist/pooler/falsification/__init__.py` & `autora-experimentalist-falsification-1.0.4/src/autora/experimentalist/pooler/falsification/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/src/autora/experimentalist/sampler/falsification/__init__.py` & `autora-experimentalist-falsification-1.0.4/src/autora/experimentalist/sampler/falsification/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Tuple, cast
+from typing import Optional, Tuple, cast, Iterable
 
 import numpy as np
 import torch
 from sklearn.preprocessing import StandardScaler
 from torch import nn
 from torch.autograd import Variable
 
@@ -119,14 +119,17 @@
 
     Returns:
         new_conditions: Samples of experimental conditions with the highest loss
         scores: Normalized falsification scores for the samples
 
     """
 
+    if isinstance(reference_conditions, Iterable):
+        reference_conditions = np.array(list(reference_conditions))
+
     reference_conditions = np.array(reference_conditions)
     if len(reference_conditions.shape) == 1:
         reference_conditions = reference_conditions.reshape(-1, 1)
 
     predicted_observations = model.predict(reference_conditions)
 
     return falsification_score_sample_from_predictions(condition_pool,
@@ -172,28 +175,36 @@
 
     Returns:
         new_conditions: Samples of experimental conditions with the highest loss
         scores: Normalized falsification scores for the samples
 
     """
 
-    X = np.array(condition_pool)
-    if len(X.shape) == 1:
-        X = X.reshape(-1, 1)
+    if isinstance(condition_pool, Iterable):
+        condition_pool = np.array(list(condition_pool))
+
+    if isinstance(condition_pool, list):
+        condition_pool = np.array(condition_pool)
+
+    if isinstance(condition_pool, np.ndarray) is False:
+        raise Exception("condition_pool must be a numpy array.")
+
+    if len(condition_pool.shape) == 1:
+        condition_pool = condition_pool.reshape(-1, 1)
 
     reference_conditions = np.array(reference_conditions)
     if len(reference_conditions.shape) == 1:
         reference_conditions = reference_conditions.reshape(-1, 1)
 
     reference_observations = np.array(reference_observations)
     if len(reference_observations.shape) == 1:
         reference_observations = reference_observations.reshape(-1, 1)
 
     if num_samples is None:
-        num_samples = X.shape[0]
+        num_samples = condition_pool.shape[0]
 
     if metadata is not None:
         if metadata.dependent_variables[0].type == ValueType.CLASS:
             # find all unique values in reference_observations
             num_classes = len(np.unique(reference_observations))
             reference_observations = class_to_onehot(reference_observations, n_classes=num_classes)
 
@@ -206,21 +217,21 @@
                                               metadata,
                                               iv_limit_list,
                                               training_epochs,
                                               training_lr,
                                               plot)
 
     # now that the popper network is trained we can assign losses to all data points to be evaluated
-    popper_input = Variable(torch.from_numpy(X)).float()
+    popper_input = Variable(torch.from_numpy(condition_pool)).float()
     Y = popper_net(popper_input).detach().numpy().flatten()
     scaler = StandardScaler()
     score = scaler.fit_transform(Y.reshape(-1, 1)).flatten()
 
     # order rows in Y from highest to lowest
-    sorted_X = X[np.argsort(score)[::-1]]
+    sorted_conditions = condition_pool[np.argsort(score)[::-1]]
     sorted_score = score[np.argsort(score)[::-1]]
 
-    return sorted_X[:num_samples], sorted_score[:num_samples]
+    return sorted_conditions[:num_samples], sorted_score[:num_samples]
 
 falsification_sampler = deprecated_alias(falsification_sample, "falsification_sampler")
 falsification_score_sampler = deprecated_alias(falsification_score_sample, "falsification_score_sampler")
 falsification_score_sampler_from_predictions = deprecated_alias(falsification_score_sample_from_predictions, "falsification_score_sampler_from_predictions")
```

### Comparing `autora-experimentalist-falsification-1.0.3/src/autora_experimentalist_falsification.egg-info/PKG-INFO` & `autora-experimentalist-falsification-1.0.4/src/autora_experimentalist_falsification.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-falsification
-Version: 1.0.3
+Version: 1.0.4
 Summary: AutoRA Falsification Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-falsification
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
```

### Comparing `autora-experimentalist-falsification-1.0.3/src/autora_experimentalist_falsification.egg-info/SOURCES.txt` & `autora-experimentalist-falsification-1.0.4/src/autora_experimentalist_falsification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/tests/README.md` & `autora-experimentalist-falsification-1.0.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/tests/test_exp_falsification_pooler.py` & `autora-experimentalist-falsification-1.0.4/tests/test_exp_falsification_pooler.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.3/tests/test_exp_falsification_sampler.py` & `autora-experimentalist-falsification-1.0.4/tests/test_exp_falsification_sampler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import pytest
 import torch
 from sklearn.linear_model import LinearRegression, LogisticRegression
 
 from autora.experimentalist.pipeline import Pipeline
+from autora.experimentalist.pooler.grid import grid_pool
 from autora.experimentalist.sampler.falsification import (
     falsification_sample,
     falsification_score_sample,
     falsification_score_sample_from_predictions,
 )
 from autora.variable import DV, IV, ValueType, VariableCollection
 from tests.test_exp_falsification_pooler import get_sin_data, get_xor_data
@@ -53,14 +54,15 @@
 
 @pytest.fixture
 def seed():
     """
     Ensures that the results are the same each time the tests are run.
     """
     torch.manual_seed(180)
+    np.random.seed(180)
     return
 
 
 @pytest.fixture
 def get_square_data():
     X = np.linspace(x_min_regression, x_max_regression, 100)
     Y = np.square(X)
@@ -72,15 +74,14 @@
     data = np.linspace(x_min_regression, x_max_regression, 11)
     return data
 
 
 def test_falsification_classification(
     synthetic_logr_model, classification_data_to_test, seed
 ):
-
     # Import model and data_closed_loop
     X_train, Y_train = get_xor_data()
     X = classification_data_to_test
     model = synthetic_logr_model
 
     # Specify independent variables
     iv1 = IV(
@@ -272,14 +273,60 @@
     # check if the scores are properly ordered
     assert scores[0] > scores[1]
 
     # check if the data points with the highest predicted error were selected
     assert np.round(X_selected[0, 0], 4) == 1.8 or np.round(X_selected[0, 0], 4) == 4.8
     assert np.round(X_selected[1, 0], 4) == 1.8 or np.round(X_selected[1, 0], 4) == 4.8
 
+def test_iterator_input(synthetic_linr_model):
+    # Import model and data_closed_loop
+    X_train, Y_train = get_sin_data()
+    model = synthetic_linr_model
+
+    # specify meta data_closed_loop
+
+    # Specify independent variables
+    iv = IV(
+        name="x",
+        value_range=(0, 2 * np.pi),
+        allowed_values=(np.linspace(0, 2 * np.pi, 100)),
+        units="intensity",
+        variable_label="stimulus",
+    )
+
+    # specify dependent variables
+    dv = DV(
+        name="y",
+        value_range=(-1, 1),
+        units="real",
+        variable_label="response",
+        type=ValueType.REAL,
+    )
+
+    # Variable collection with ivs and dvs
+    metadata = VariableCollection(
+        independent_variables=[iv],
+        dependent_variables=[dv],
+    )
+
+    X = grid_pool(metadata.independent_variables)
+
+    new_conditions, new_scores = falsification_score_sample(
+                condition_pool=X,
+                model=model,
+                reference_conditions=X_train,
+                reference_observations=Y_train,
+                metadata=metadata,
+                num_samples=5,
+                training_epochs=1000,
+                training_lr=1e-3,
+                plot=False,
+            )
+
+    assert new_conditions.shape[0] == 5
 
 def test_doc_example():
     # Specify X and Y
     X = np.linspace(0, 2 * np.pi, 100)
     Y = np.sin(X)
     X_prime = np.linspace(0, 6.5, 14)
```

