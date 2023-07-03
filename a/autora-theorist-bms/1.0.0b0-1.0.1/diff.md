# Comparing `tmp/autora-theorist-bms-1.0.0b0.tar.gz` & `tmp/autora-theorist-bms-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-bms-1.0.0b0.tar", last modified: Thu May 11 15:54:07 2023, max compression
+gzip compressed data, was "autora-theorist-bms-1.0.1.tar", last modified: Mon Jul  3 18:48:39 2023, max compression
```

## Comparing `autora-theorist-bms-1.0.0b0.tar` & `autora-theorist-bms-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    34238 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/how-it-works.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   191653 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/img/BMSEquationTreeOps.png
--rw-r--r--   0 runner    (1001) docker     (123)   503083 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/img/BMSTempering.png
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/meta-parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/docs/search-space.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.396622 autora-theorist-bms-1.0.0b0/src/autora/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.400622 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/fit_prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    60423 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/regressor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2860 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 15:54:07.000000 autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:54:07.404622 autora-theorist-bms-1.0.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-05-11 15:53:54.000000 autora-theorist-bms-1.0.0b0/tests/test_sklearn_bms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.852536 autora-theorist-bms-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.840536 autora-theorist-bms-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 18:48:39.848536 autora-theorist-bms-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    34190 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/how-it-works.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   191653 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/img/BMSEquationTreeOps.png
+-rw-r--r--   0 runner    (1001) docker     (123)   503083 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/img/BMSTempering.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/meta-parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/docs/search-space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.844536 autora-theorist-bms-1.0.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 18:48:39.852536 autora-theorist-bms-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.840536 autora-theorist-bms-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.840536 autora-theorist-bms-1.0.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.840536 autora-theorist-bms-1.0.1/src/autora/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.848536 autora-theorist-bms-1.0.1/src/autora/theorist/bms/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/fit_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60423 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/regressor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2860 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/src/autora/theorist/bms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.848536 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 18:48:39.000000 autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:39.848536 autora-theorist-bms-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-07-03 18:48:26.000000 autora-theorist-bms-1.0.1/tests/test_sklearn_bms.py
```

### Comparing `autora-theorist-bms-1.0.0b0/.github/workflows/python-publish.yml` & `autora-theorist-bms-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/.gitignore` & `autora-theorist-bms-1.0.1/.gitignore`

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

### Comparing `autora-theorist-bms-1.0.0b0/.pre-commit-config.yaml` & `autora-theorist-bms-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/docs/basic-usage.ipynb` & `autora-theorist-bms-1.0.1/docs/Basic Usage.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Basic Usage\\n')], delete: [0]}, 'attachments': "*

 * *            "OrderedDict()}, 1: {'source': {insert: [(1, '# !pip install "*

 * *            '"autora[theorist-bms]"\')], delete: [1]}}, 11: {\'outputs\': {0: {\'data\': '*

 * *            "{'text/plain': ['<Figure size 640x480 with 1 Axes>']}}}, 'source': {insert: [(5, "*

 * *            "'bms_estimator.model_.latex()')]}}, delete: [0]}"}*

```diff
@@ -1,39 +1,31 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "# Bayesian Machine Scientist"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {
-                "collapsed": false
-            },
-            "source": [
-                "## Basic Example\n",
+                "# Basic Usage\n",
                 "\n",
                 "The following simple example shows out-of-the-box functionality of BMS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "# Uncomment the following line when running on Google Colab\n",
-                "# !pip install autora"
+                "# !pip install \"autora[theorist-bms]\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
@@ -146,26 +138,29 @@
             "metadata": {
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
-                        "text/plain": "<Figure size 640x480 with 1 Axes>"
+                        "text/plain": [
+                            "<Figure size 640x480 with 1 Axes>"
+                        ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# plot out the ground truth versus predicted responses\n",
                 "plt.figure()\n",
                 "plt.plot(x, y, \"o\")\n",
                 "plt.plot(x, y_pred, \"-\")\n",
-                "plt.show()"
+                "plt.show()",
+                "bms_estimator.model_.latex()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
```

### Comparing `autora-theorist-bms-1.0.0b0/docs/how-it-works.md` & `autora-theorist-bms-1.0.1/docs/how-it-works.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# Bayesian Machine Scientist
-
-## How it works
+# How It Works
 
 The Bayesian Machine Scientist (BMS) uses Bayesian inference to search the space of possible equations. The following are the relevant quantities in this Bayesian approach:
 
 - $P(x):$ Probability of $x$
 - $P(x|\theta)$: Conditional Probability of $x$ given $\theta$
 - $P(x,\theta)$: Joint Probability of $x$ and $\theta$
```

### Comparing `autora-theorist-bms-1.0.0b0/docs/img/BMSEquationTreeOps.png` & `autora-theorist-bms-1.0.1/docs/img/BMSEquationTreeOps.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/docs/img/BMSTempering.png` & `autora-theorist-bms-1.0.1/docs/img/BMSTempering.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/docs/index.md` & `autora-theorist-bms-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/docs/meta-parameters.md` & `autora-theorist-bms-1.0.1/docs/meta-parameters.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Bayesian Machine Scientist
+# Meta Parameters
 
-## Meta-Parameters
-
-Meta-parameters are used to control the search space and the search algorithm. This section provides a basic overview of these parameters along with a description of their effects. 
+Meta parameters are used to control the search space and the search algorithm. This section provides a basic overview of these parameters along with a description of their effects. 
 
 - **`epochs`**: The number of epochs to run BMS. This corresponds to the total number of equation mutations - one mcmc step for each parallel-tempered equation and one tree swap between a pair of parallel-tempered equations.
 - **`prior_par`**: A dictionary of priors for each operation. The keys correspond to operations and the respective values correspond to prior probabilities of those operations. The model comes with a default.  
 - **`ts`**: A list of temperature values. The machine scientist creates an equation tree for each of these values. Higher temperature trees are harder to fit, and thus they help prevent overfitting of the model.
```

### Comparing `autora-theorist-bms-1.0.0b0/mkdocs/base.yml` & `autora-theorist-bms-1.0.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/pyproject.toml` & `autora-theorist-bms-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/fit_prior.py` & `autora-theorist-bms-1.0.1/src/autora/theorist/bms/fit_prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/mcmc.py` & `autora-theorist-bms-1.0.1/src/autora/theorist/bms/mcmc.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/parallel.py` & `autora-theorist-bms-1.0.1/src/autora/theorist/bms/parallel.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/prior.py` & `autora-theorist-bms-1.0.1/src/autora/theorist/bms/prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/regressor.py` & `autora-theorist-bms-1.0.1/src/autora/theorist/bms/regressor.py`

 * *Files 9% similar despite different names*

```diff
@@ -170,11 +170,17 @@
         check_is_fitted(self, attributes=["model_", "loss_", "cache_"])
         assert self.model_ is not None
         assert self.loss_ is not None
         assert self.cache_ is not None
 
         utils.present_results(self.model_, self.loss_, self.cache_)
 
+    def repr(self):
+        return self.model_.__repr__()
+
+    def latex(self):
+        return self.model_.latex()
+
     def add_primitive(self, op: Callable):
         self.custom_ops.update({op.__name__: op})
         self.ops.update({op.__name__: len(signature(op).parameters)})
         self.prior_par.update({"Nopi_" + op.__name__: 1})
```

### Comparing `autora-theorist-bms-1.0.0b0/src/autora/theorist/bms/utils.py` & `autora-theorist-bms-1.0.1/src/autora/theorist/bms/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/src/autora_theorist_bms.egg-info/SOURCES.txt` & `autora-theorist-bms-1.0.1/src/autora_theorist_bms.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/python-publish.yml
-docs/basic-usage.ipynb
+docs/Basic Usage.ipynb
 docs/how-it-works.md
 docs/index.md
 docs/meta-parameters.md
 docs/quickstart.md
-docs/search-space.ipynb
+docs/search-space.md
 docs/img/BMSEquationTreeOps.png
 docs/img/BMSTempering.png
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 src/autora/theorist/bms/__init__.py
 src/autora/theorist/bms/fit_prior.py
 src/autora/theorist/bms/mcmc.py
```

### Comparing `autora-theorist-bms-1.0.0b0/tests/README.md` & `autora-theorist-bms-1.0.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bms-1.0.0b0/tests/test_sklearn_bms.py` & `autora-theorist-bms-1.0.1/tests/test_sklearn_bms.py`

 * *Files identical despite different names*
