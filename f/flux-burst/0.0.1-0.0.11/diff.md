# Comparing `tmp/flux-burst-0.0.1.tar.gz` & `tmp/flux-burst-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-0.0.1.tar", last modified: Sat Jul  1 06:52:49 2023, max compression
+gzip compressed data, was "flux-burst-0.0.11.tar", last modified: Mon Jul  3 07:22:13 2023, max compression
```

## Comparing `flux-burst-0.0.1.tar` & `flux-burst-0.0.11.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.1/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.1/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.1/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.1/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4499 2023-07-01 06:52:49.261483 flux-burst-0.0.1/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3662 2023-06-25 21:04:01.000000 flux-burst-0.0.1/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/flux_burst.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4499 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      723 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.1/flux_burst.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-01 06:52:49.000000 flux-burst-0.0.1/flux_burst.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/fluxburst/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.1/fluxburst/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7997 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/defaults.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/fluxburst/kubernetes/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/kubernetes/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/kubernetes/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/kubernetes/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6537 2023-07-01 06:52:00.000000 flux-burst-0.0.1/fluxburst/kubernetes/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.1/fluxburst/logger.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2430 2023-06-30 06:24:43.000000 flux-burst-0.0.1/fluxburst/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-06-24 04:45:23.000000 flux-burst-0.0.1/fluxburst/selectors.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.1/fluxburst/sorting.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-01 06:52:49.261483 flux-burst-0.0.1/fluxburst/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      540 2023-06-23 19:26:33.000000 flux-burst-0.0.1/fluxburst/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-06-23 19:45:55.000000 flux-burst-0.0.1/fluxburst/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1692 2023-06-23 19:41:30.000000 flux-burst-0.0.1/fluxburst/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.1/fluxburst/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1262 2023-07-01 06:52:09.000000 flux-burst-0.0.1/fluxburst/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.1/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-01 06:52:49.261483 flux-burst-0.0.1/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.1/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.11/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.11/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.11/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.11/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-03 07:22:13.278146 flux-burst-0.0.11/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3880 2023-07-03 07:21:31.000000 flux-burst-0.0.11/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/flux_burst.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      744 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.11/flux_burst.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-03 07:22:13.000000 flux-burst-0.0.11/flux_burst.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/fluxburst/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.11/fluxburst/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7109 2023-07-03 07:21:31.000000 flux-burst-0.0.11/fluxburst/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7534 2023-07-03 07:21:31.000000 flux-burst-0.0.11/fluxburst/handles.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/fluxburst/kubernetes/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/kubernetes/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/kubernetes/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/kubernetes/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6537 2023-07-01 06:52:00.000000 flux-burst-0.0.11/fluxburst/kubernetes/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.11/fluxburst/logger.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2831 2023-07-03 07:21:31.000000 flux-burst-0.0.11/fluxburst/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-06-24 04:45:23.000000 flux-burst-0.0.11/fluxburst/selectors.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.11/fluxburst/sorting.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-03 07:22:13.278146 flux-burst-0.0.11/fluxburst/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      540 2023-06-23 19:26:33.000000 flux-burst-0.0.11/fluxburst/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-06-23 19:45:55.000000 flux-burst-0.0.11/fluxburst/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1692 2023-06-23 19:41:30.000000 flux-burst-0.0.11/fluxburst/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.11/fluxburst/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1263 2023-07-03 07:22:00.000000 flux-burst-0.0.11/fluxburst/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.11/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-03 07:22:13.278146 flux-burst-0.0.11/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.11/setup.py
```

### Comparing `flux-burst-0.0.1/LICENSE` & `flux-burst-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/NOTICE` & `flux-burst-0.0.11/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/PKG-INFO` & `flux-burst-0.0.11/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.1
+Version: 0.0.11
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
@@ -57,14 +57,16 @@
 - We need a reasonable default for what a plugin should do if something fails (e.g., setup/config)
 - How should each plugin decide what size cluster to make? Right now I'm just taking the max size of the job, and we are assuming the jobs need the same node type.
 - We will eventually want to use namespaces in a meaningful way (e.g., users)
 - We will eventually want a specific burst for a job to be able to customize in more detail, e.g., the namespace or other attribute that comes from a jobspec (right now they are global to the plugin)
 - Who controls cleanup? It can be done by the flux-burst global controller or a plugin, automated or manual, either way.
 - All plugins should have support to read in YAML parameters (some spec for bursting)
 - All plugins should be able to match a resource request to, for example, instance types.
+- Should the plugin "local queue" (self.jobs) assume to be associated with one burst, where the size is the max job size?
+- Should we derive names based on provided name + size so clusters are unique by name and size?
 
 ## 😁️ Contributors 😁️
 
 We use the [all-contributors](https://github.com/all-contributors/all-contributors)
 tool to generate a contributors graphic below.
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,46 +1,49 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.1 Summary: Flux module that
-enables burstable plugins. Home-page: https://github.com/converged-computing/
-flux-burst Author: Vanessa Sochat Author-email: vsoch@users.noreply.github.com
-Maintainer: Vanessa Sochat License: LICENSE Keywords: cloud,flux-
-framework,flux,bursting Platform: UNKNOWN Classifier: Intended Audience ::
-Science/Research Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python Classifier: Topic :: Software Development Classifier: Topic ::
-Scientific/Engineering Classifier: Operating System :: Unix Classifier:
-Programming Language :: Python :: 3.8 Description-Content-Type: text/markdown
-Provides-Extra: all Provides-Extra: kubernetes License-File: LICENSE License-
-File: NOTICE # Flux Burst  [![All Contributors](https://img.shields.io/badge/
-all_contributors-1-orange.svg?style=flat-square)](#contributors-)  [![PyPI]
-(https://img.shields.io/pypi/v/flux-burst)](https://pypi.org/project/flux-
-burst/)  ![https://raw.githubusercontent.com/converged-computing/flux-burst/
-main/docs/assets/img/logo.png](https://raw.githubusercontent.com/converged-
-computing/flux-burst/main/docs/assets/img/logo.png) This is a Python module to
-coordinate Flux bursting. ð§ï¸ - â­ï¸ [Documentation](https://converged-
-computing.github.io/flux-burst/) â­ï¸ - ð¦ï¸ [Pypi Package](https://
-pypi.org/project/flux-burst/) ð¦ï¸ ## Plugins Current and desired plugins
-are: - [local mock](https://github.com/flux-framework/flux-sched/issues/
-1009#issuecomment-1603636498) - [Google Cloud](https://github.com/converged-
-computing/flux-burst-gke) - AWS (not written yet) ## Questions - How should the
-plugins (or client) manage checking when to create / destroy clusters? - Can we
-have a better strategy for namespacing different bursts (e.g., beyond burst-0,
-burst-1, ..., burst-N) - We need a reasonable default for what a plugin should
-do if something fails (e.g., setup/config) - How should each plugin decide what
-size cluster to make? Right now I'm just taking the max size of the job, and we
-are assuming the jobs need the same node type. - We will eventually want to use
-namespaces in a meaningful way (e.g., users) - We will eventually want a
-specific burst for a job to be able to customize in more detail, e.g., the
-namespace or other attribute that comes from a jobspec (right now they are
-global to the plugin) - Who controls cleanup? It can be done by the flux-burst
-global controller or a plugin, automated or manual, either way. - All plugins
-should have support to read in YAML parameters (some spec for bursting) - All
-plugins should be able to match a resource request to, for example, instance
-types. ## ðï¸ Contributors ðï¸ We use the [all-contributors](https://
-github.com/all-contributors/all-contributors) tool to generate a contributors
-graphic below.
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.11 Summary: Flux module
+that enables burstable plugins. Home-page: https://github.com/converged-
+computing/flux-burst Author: Vanessa Sochat Author-email:
+vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
+Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
+Intended Audience :: Science/Research Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
+Unix Classifier: Programming Language :: Python :: 3.8 Description-Content-
+Type: text/markdown Provides-Extra: all Provides-Extra: kubernetes License-
+File: LICENSE License-File: NOTICE # Flux Burst  [![All Contributors](https://
+img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)]
+(#contributors-)  [![PyPI](https://img.shields.io/pypi/v/flux-burst)](https://
+pypi.org/project/flux-burst/)  ![https://raw.githubusercontent.com/converged-
+computing/flux-burst/main/docs/assets/img/logo.png](https://
+raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/
+logo.png) This is a Python module to coordinate Flux bursting. ð§ï¸ - â­ï¸
+[Documentation](https://converged-computing.github.io/flux-burst/) â­ï¸ -
+ð¦ï¸ [Pypi Package](https://pypi.org/project/flux-burst/) ð¦ï¸ ## Plugins
+Current and desired plugins are: - [local mock](https://github.com/flux-
+framework/flux-sched/issues/1009#issuecomment-1603636498) - [Google Cloud]
+(https://github.com/converged-computing/flux-burst-gke) - AWS (not written yet)
+## Questions - How should the plugins (or client) manage checking when to
+create / destroy clusters? - Can we have a better strategy for namespacing
+different bursts (e.g., beyond burst-0, burst-1, ..., burst-N) - We need a
+reasonable default for what a plugin should do if something fails (e.g., setup/
+config) - How should each plugin decide what size cluster to make? Right now
+I'm just taking the max size of the job, and we are assuming the jobs need the
+same node type. - We will eventually want to use namespaces in a meaningful way
+(e.g., users) - We will eventually want a specific burst for a job to be able
+to customize in more detail, e.g., the namespace or other attribute that comes
+from a jobspec (right now they are global to the plugin) - Who controls
+cleanup? It can be done by the flux-burst global controller or a plugin,
+automated or manual, either way. - All plugins should have support to read in
+YAML parameters (some spec for bursting) - All plugins should be able to match
+a resource request to, for example, instance types. - Should the plugin "local
+queue" (self.jobs) assume to be associated with one burst, where the size is
+the max job size? - Should we derive names based on provided name + size so
+clusters are unique by name and size? ## ðï¸ Contributors ðï¸ We use
+the [all-contributors](https://github.com/all-contributors/all-contributors)
+tool to generate a contributors graphic below.
 [Vanessasaurus]
  Vanessasaurus
      ð»
    ## License HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license. See [LICENSE](https://
 github.com/converged-computing/flux-burst/blob/main/LICENSE), [COPYRIGHT]
 (https://github.com/converged-computing/flux-burst/blob/main/COPYRIGHT), and
```

### Comparing `flux-burst-0.0.1/README.md` & `flux-burst-0.0.11/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 - We need a reasonable default for what a plugin should do if something fails (e.g., setup/config)
 - How should each plugin decide what size cluster to make? Right now I'm just taking the max size of the job, and we are assuming the jobs need the same node type.
 - We will eventually want to use namespaces in a meaningful way (e.g., users)
 - We will eventually want a specific burst for a job to be able to customize in more detail, e.g., the namespace or other attribute that comes from a jobspec (right now they are global to the plugin)
 - Who controls cleanup? It can be done by the flux-burst global controller or a plugin, automated or manual, either way.
 - All plugins should have support to read in YAML parameters (some spec for bursting)
 - All plugins should be able to match a resource request to, for example, instance types.
+- Should the plugin "local queue" (self.jobs) assume to be associated with one burst, where the size is the max job size?
+- Should we derive names based on provided name + size so clusters are unique by name and size?
 
 ## 😁️ Contributors 😁️
 
 We use the [all-contributors](https://github.com/all-contributors/all-contributors)
 tool to generate a contributors graphic below.
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -19,17 +19,20 @@
 namespaces in a meaningful way (e.g., users) - We will eventually want a
 specific burst for a job to be able to customize in more detail, e.g., the
 namespace or other attribute that comes from a jobspec (right now they are
 global to the plugin) - Who controls cleanup? It can be done by the flux-burst
 global controller or a plugin, automated or manual, either way. - All plugins
 should have support to read in YAML parameters (some spec for bursting) - All
 plugins should be able to match a resource request to, for example, instance
-types. ## ðï¸ Contributors ðï¸ We use the [all-contributors](https://
-github.com/all-contributors/all-contributors) tool to generate a contributors
-graphic below.
+types. - Should the plugin "local queue" (self.jobs) assume to be associated
+with one burst, where the size is the max job size? - Should we derive names
+based on provided name + size so clusters are unique by name and size? ##
+ðï¸ Contributors ðï¸ We use the [all-contributors](https://github.com/
+all-contributors/all-contributors) tool to generate a contributors graphic
+below.
 [Vanessasaurus]
  Vanessasaurus
      ð»
    ## License HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license. See [LICENSE](https://
 github.com/converged-computing/flux-burst/blob/main/LICENSE), [COPYRIGHT]
 (https://github.com/converged-computing/flux-burst/blob/main/COPYRIGHT), and
```

### Comparing `flux-burst-0.0.1/flux_burst.egg-info/PKG-INFO` & `flux-burst-0.0.11/flux_burst.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.1
+Version: 0.0.11
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
@@ -57,14 +57,16 @@
 - We need a reasonable default for what a plugin should do if something fails (e.g., setup/config)
 - How should each plugin decide what size cluster to make? Right now I'm just taking the max size of the job, and we are assuming the jobs need the same node type.
 - We will eventually want to use namespaces in a meaningful way (e.g., users)
 - We will eventually want a specific burst for a job to be able to customize in more detail, e.g., the namespace or other attribute that comes from a jobspec (right now they are global to the plugin)
 - Who controls cleanup? It can be done by the flux-burst global controller or a plugin, automated or manual, either way.
 - All plugins should have support to read in YAML parameters (some spec for bursting)
 - All plugins should be able to match a resource request to, for example, instance types.
+- Should the plugin "local queue" (self.jobs) assume to be associated with one burst, where the size is the max job size?
+- Should we derive names based on provided name + size so clusters are unique by name and size?
 
 ## 😁️ Contributors 😁️
 
 We use the [all-contributors](https://github.com/all-contributors/all-contributors)
 tool to generate a contributors graphic below.
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,46 +1,49 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.1 Summary: Flux module that
-enables burstable plugins. Home-page: https://github.com/converged-computing/
-flux-burst Author: Vanessa Sochat Author-email: vsoch@users.noreply.github.com
-Maintainer: Vanessa Sochat License: LICENSE Keywords: cloud,flux-
-framework,flux,bursting Platform: UNKNOWN Classifier: Intended Audience ::
-Science/Research Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python Classifier: Topic :: Software Development Classifier: Topic ::
-Scientific/Engineering Classifier: Operating System :: Unix Classifier:
-Programming Language :: Python :: 3.8 Description-Content-Type: text/markdown
-Provides-Extra: all Provides-Extra: kubernetes License-File: LICENSE License-
-File: NOTICE # Flux Burst  [![All Contributors](https://img.shields.io/badge/
-all_contributors-1-orange.svg?style=flat-square)](#contributors-)  [![PyPI]
-(https://img.shields.io/pypi/v/flux-burst)](https://pypi.org/project/flux-
-burst/)  ![https://raw.githubusercontent.com/converged-computing/flux-burst/
-main/docs/assets/img/logo.png](https://raw.githubusercontent.com/converged-
-computing/flux-burst/main/docs/assets/img/logo.png) This is a Python module to
-coordinate Flux bursting. ð§ï¸ - â­ï¸ [Documentation](https://converged-
-computing.github.io/flux-burst/) â­ï¸ - ð¦ï¸ [Pypi Package](https://
-pypi.org/project/flux-burst/) ð¦ï¸ ## Plugins Current and desired plugins
-are: - [local mock](https://github.com/flux-framework/flux-sched/issues/
-1009#issuecomment-1603636498) - [Google Cloud](https://github.com/converged-
-computing/flux-burst-gke) - AWS (not written yet) ## Questions - How should the
-plugins (or client) manage checking when to create / destroy clusters? - Can we
-have a better strategy for namespacing different bursts (e.g., beyond burst-0,
-burst-1, ..., burst-N) - We need a reasonable default for what a plugin should
-do if something fails (e.g., setup/config) - How should each plugin decide what
-size cluster to make? Right now I'm just taking the max size of the job, and we
-are assuming the jobs need the same node type. - We will eventually want to use
-namespaces in a meaningful way (e.g., users) - We will eventually want a
-specific burst for a job to be able to customize in more detail, e.g., the
-namespace or other attribute that comes from a jobspec (right now they are
-global to the plugin) - Who controls cleanup? It can be done by the flux-burst
-global controller or a plugin, automated or manual, either way. - All plugins
-should have support to read in YAML parameters (some spec for bursting) - All
-plugins should be able to match a resource request to, for example, instance
-types. ## ðï¸ Contributors ðï¸ We use the [all-contributors](https://
-github.com/all-contributors/all-contributors) tool to generate a contributors
-graphic below.
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.11 Summary: Flux module
+that enables burstable plugins. Home-page: https://github.com/converged-
+computing/flux-burst Author: Vanessa Sochat Author-email:
+vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
+Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
+Intended Audience :: Science/Research Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
+Unix Classifier: Programming Language :: Python :: 3.8 Description-Content-
+Type: text/markdown Provides-Extra: all Provides-Extra: kubernetes License-
+File: LICENSE License-File: NOTICE # Flux Burst  [![All Contributors](https://
+img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)]
+(#contributors-)  [![PyPI](https://img.shields.io/pypi/v/flux-burst)](https://
+pypi.org/project/flux-burst/)  ![https://raw.githubusercontent.com/converged-
+computing/flux-burst/main/docs/assets/img/logo.png](https://
+raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/
+logo.png) This is a Python module to coordinate Flux bursting. ð§ï¸ - â­ï¸
+[Documentation](https://converged-computing.github.io/flux-burst/) â­ï¸ -
+ð¦ï¸ [Pypi Package](https://pypi.org/project/flux-burst/) ð¦ï¸ ## Plugins
+Current and desired plugins are: - [local mock](https://github.com/flux-
+framework/flux-sched/issues/1009#issuecomment-1603636498) - [Google Cloud]
+(https://github.com/converged-computing/flux-burst-gke) - AWS (not written yet)
+## Questions - How should the plugins (or client) manage checking when to
+create / destroy clusters? - Can we have a better strategy for namespacing
+different bursts (e.g., beyond burst-0, burst-1, ..., burst-N) - We need a
+reasonable default for what a plugin should do if something fails (e.g., setup/
+config) - How should each plugin decide what size cluster to make? Right now
+I'm just taking the max size of the job, and we are assuming the jobs need the
+same node type. - We will eventually want to use namespaces in a meaningful way
+(e.g., users) - We will eventually want a specific burst for a job to be able
+to customize in more detail, e.g., the namespace or other attribute that comes
+from a jobspec (right now they are global to the plugin) - Who controls
+cleanup? It can be done by the flux-burst global controller or a plugin,
+automated or manual, either way. - All plugins should have support to read in
+YAML parameters (some spec for bursting) - All plugins should be able to match
+a resource request to, for example, instance types. - Should the plugin "local
+queue" (self.jobs) assume to be associated with one burst, where the size is
+the max job size? - Should we derive names based on provided name + size so
+clusters are unique by name and size? ## ðï¸ Contributors ðï¸ We use
+the [all-contributors](https://github.com/all-contributors/all-contributors)
+tool to generate a contributors graphic below.
 [Vanessasaurus]
  Vanessasaurus
      ð»
    ## License HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license. See [LICENSE](https://
 github.com/converged-computing/flux-burst/blob/main/LICENSE), [COPYRIGHT]
 (https://github.com/converged-computing/flux-burst/blob/main/COPYRIGHT), and
```

### Comparing `flux-burst-0.0.1/flux_burst.egg-info/SOURCES.txt` & `flux-burst-0.0.11/flux_burst.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 flux_burst.egg-info/entry_points.txt
 flux_burst.egg-info/not-zip-safe
 flux_burst.egg-info/requires.txt
 flux_burst.egg-info/top_level.txt
 fluxburst/__init__.py
 fluxburst/client.py
 fluxburst/defaults.py
+fluxburst/handles.py
 fluxburst/logger.py
 fluxburst/plugins.py
 fluxburst/selectors.py
 fluxburst/sorting.py
 fluxburst/version.py
 fluxburst/kubernetes/README.md
 fluxburst/kubernetes/__init__.py
```

### Comparing `flux-burst-0.0.1/fluxburst/client.py` & `flux-burst-0.0.11/fluxburst/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
 import collections
 
-import flux
-import flux.job
-
+import fluxburst.handles as handles
 import fluxburst.selectors as selectors
 import fluxburst.sorting as sorting
 from fluxburst.logger import logger
 
 from .plugins import burstable_plugins
 
 
 class FluxBurst:
     """
     Flux Burst Client
     """
 
-    def __init__(self, handle=None):
+    def __init__(self, handle=None, mock=False):
         """
         Create a new burst client.
 
         Selectors: Process the current queue and add flags/filter jobs for plugins.
         Plugins: take jobs that need bursting, and burst some subset.
         A filter can (on the simplest terms) just look for a job flagged as
         burstable. For more complex cases, it can perform it's own logic and
         flag some subset as burstable instead.
         """
         self.reset_selector()
         self.reset_plugins()
-        self.handle = handle or flux.Flux()
+        self.flux = handles.FluxMock(handle) if mock else handles.FluxHandle(handle)
         self.set_ordering(sorting.in_order)
 
     @property
     def choices(self):
         return "|".join(list(self.plugins))
 
     def load(self, name, dataclass, **kwargs):
@@ -171,62 +169,37 @@
 
         # The job is no longer marked as burstable for other plugins
         if "burstable" in job["spec"]["attributes"]["system"]:
             del job["spec"]["attributes"]["system"]["burstable"]
 
         # Update the KVS (is this possible)?
         # This doesn't currently work, so not doing anything :)
-        kvs = flux.job.job_kvs(self.handle, job["id"])
-        kvs["jobspec"] = job["spec"]
-        kvs.commit()
+        self.flux.update_jobspec(job)
 
     def select_jobs(self):
         """
         Use filters to select jobs.
 
         This step is agnostic to the burstable plugins - it is simply
         deducing (via our selector function) what jobs are contenders
         for bursting. See the README / documentation for example info.
         """
         # Keep track of selected burstable jobs by id
-        listing = flux.job.job_list(self.handle).get()
+        listing = self.flux.list_jobs()
         selected = {}
 
         for job in listing.get("jobs", []):
-            info = self.get_job_info(job["id"])
+            info = self.flux.get_job_info(job["id"])
             if not self._job_selector(info):
                 continue
             print(f"🧋️  Job {job['id']} is marked for bursting.")
             selected[job["id"]] = info
 
         # We don't give a warning here, because likely there aren't
         # jobs that are burstable (it's a more rare event)
         return selected
 
     def __repr__(self):
         return str(self)
 
     def __str__(self):
         return "[flux-burst-client]"
-
-    def get_job_info(self, jobid):
-        """
-        Get job info based on an id
-
-        Also retrieve the full job info and jobspec.
-        This is not yet currently perfectly json serializable, need to
-        handle EmptyObject if that is desired.
-        """
-        fluxjob = flux.job.JobID(jobid)
-        payload = {"id": fluxjob, "attrs": ["all"]}
-        rpc = flux.job.list.JobListIdRPC(self.handle, "job-list.list-id", payload)
-        job = rpc.get_job()
-
-        # Job info, timing, priority, etc.
-        job["info"] = rpc.get_jobinfo().__dict__
-        job["info"]["_exception"] = job["info"]["_exception"].__dict__
-        job["info"]["_annotations"] = job["info"]["_annotations"].__dict__
-
-        # the KVS will have annotations!
-        kvs = flux.job.job_kvs(self.handle, jobid)
-        job["spec"] = kvs.get("jobspec")
-        return job
```

### Comparing `flux-burst-0.0.1/fluxburst/defaults.py` & `flux-burst-0.0.11/fluxburst/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/fluxburst/kubernetes/cluster.py` & `flux-burst-0.0.11/fluxburst/kubernetes/cluster.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/fluxburst/kubernetes/plugins.py` & `flux-burst-0.0.11/fluxburst/kubernetes/plugins.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/fluxburst/logger.py` & `flux-burst-0.0.11/fluxburst/logger.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/fluxburst/plugins.py` & `flux-burst-0.0.11/fluxburst/plugins.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,29 +32,43 @@
 
     # Default dataclass is essentially empty
     _param_dataclass = BurstParameters
 
     def __init__(self, dataclass, **kwargs):
         self.set_params(dataclass)
 
-        # Set of jobs assigned to be bursted
+        # Set of jobs assigned to be bursted, and bursted clusters
         self.jobs = {}
+        self.clusters = {}
 
     def schedule(self, job):
         """
         Attempt to schedule a job, if possible.
         """
         raise NotImplementedError
 
     def run(self, *args, **kwargs):
         """
         Main function to run a plugin with the set of burstable jobs.
         """
         raise NotImplementedError
 
+    def cleanup(self, name=None):
+        pass
+
+    def refresh_clusters(self, clusters):
+        """
+        Update known clusters from a list of those removed.
+        """
+        updated = {}
+        for name in self.clusters:
+            if name not in clusters:
+                updated[name] = self.clusters[name]
+        self.clusters = updated
+
     def set_params(self, dc):
         """
         Given known parameters, assert we have the correct dataclass
         and update from the environment, etc.
 
         The dc (dataclass) is used by the plugin as a generic strategy
         to select and move around custom arguments, if needed.
```

### Comparing `flux-burst-0.0.1/fluxburst/utils/__init__.py` & `flux-burst-0.0.11/fluxburst/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/fluxburst/utils/fileio.py` & `flux-burst-0.0.11/fluxburst/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/fluxburst/utils/misc.py` & `flux-burst-0.0.11/fluxburst/utils/misc.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/fluxburst/utils/terminal.py` & `flux-burst-0.0.11/fluxburst/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.1/fluxburst/version.py` & `flux-burst-0.0.11/fluxburst/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.1"
+__version__ = "0.0.11"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst"
 KEYWORDS = "cloud, flux-framework, flux, bursting"
 DESCRIPTION = "Flux module that enables burstable plugins."
 LICENSE = "LICENSE"
```

### Comparing `flux-burst-0.0.1/setup.py` & `flux-burst-0.0.11/setup.py`

 * *Files identical despite different names*

