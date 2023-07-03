# Comparing `tmp/pants-plugin-dep-graph-1.0.2.tar.gz` & `tmp/pants-plugin-dep-graph-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pants-plugin-dep-graph-1.0.2.tar", last modified: Sat Jun 24 14:52:26 2023, max compression
+gzip compressed data, was "pants-plugin-dep-graph-1.0.3.tar", last modified: Mon Jul  3 15:20:22 2023, max compression
```

## Comparing `pants-plugin-dep-graph-1.0.2.tar` & `pants-plugin-dep-graph-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-06-24 14:52:26.953881 pants-plugin-dep-graph-1.0.2/
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)       12 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/MANIFEST.in
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      945 2023-06-24 14:52:26.953881 pants-plugin-dep-graph-1.0.2/PKG-INFO
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      749 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/backend_shim.py
-drwxr-xr-x   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-06-24 14:52:26.952881 pants-plugin-dep-graph-1.0.2/depgraph/
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/depgraph/__init__.py
-drwxr-xr-x   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-06-24 14:52:26.952881 pants-plugin-dep-graph-1.0.2/depgraph/backend/
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/depgraph/backend/__init__.py
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)     2016 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/depgraph/backend/goal.py
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)     4356 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/depgraph/backend/rules.py
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      633 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/depgraph/backend/structs.py
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      231 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/depgraph/register.py
-drwxr-xr-x   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-06-24 14:52:26.952881 pants-plugin-dep-graph-1.0.2/pants_plugin_dep_graph.egg-info/
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      945 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/pants_plugin_dep_graph.egg-info/PKG-INFO
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      519 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/pants_plugin_dep_graph.egg-info/SOURCES.txt
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        1 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/pants_plugin_dep_graph.egg-info/dependency_links.txt
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)       98 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/pants_plugin_dep_graph.egg-info/entry_points.txt
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        1 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/pants_plugin_dep_graph.egg-info/namespace_packages.txt
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)       33 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/pants_plugin_dep_graph.egg-info/requires.txt
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        9 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/pants_plugin_dep_graph.egg-info/top_level.txt
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)       38 2023-06-24 14:52:26.953881 pants-plugin-dep-graph-1.0.2/setup.cfg
--rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)     1514 2023-06-24 14:52:26.000000 pants-plugin-dep-graph-1.0.2/setup.py
+drwxr-xr-x   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-07-03 15:20:22.880759 pants-plugin-dep-graph-1.0.3/
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)       12 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/MANIFEST.in
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)     1256 2023-07-03 15:20:22.880759 pants-plugin-dep-graph-1.0.3/PKG-INFO
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      749 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/backend_shim.py
+drwxr-xr-x   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-07-03 15:20:22.880759 pants-plugin-dep-graph-1.0.3/depgraph/
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/depgraph/__init__.py
+drwxr-xr-x   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-07-03 15:20:22.880759 pants-plugin-dep-graph-1.0.3/depgraph/backend/
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/depgraph/backend/__init__.py
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)     2016 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/depgraph/backend/goal.py
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)     4356 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/depgraph/backend/rules.py
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      633 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/depgraph/backend/structs.py
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      231 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/depgraph/register.py
+drwxr-xr-x   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        0 2023-07-03 15:20:22.880759 pants-plugin-dep-graph-1.0.3/pants_plugin_dep_graph.egg-info/
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)     1256 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/pants_plugin_dep_graph.egg-info/PKG-INFO
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)      519 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/pants_plugin_dep_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        1 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/pants_plugin_dep_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)       98 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/pants_plugin_dep_graph.egg-info/entry_points.txt
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        1 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/pants_plugin_dep_graph.egg-info/namespace_packages.txt
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)       33 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/pants_plugin_dep_graph.egg-info/requires.txt
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)        9 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/pants_plugin_dep_graph.egg-info/top_level.txt
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)       38 2023-07-03 15:20:22.880759 pants-plugin-dep-graph-1.0.3/setup.cfg
+-rw-r--r--   0 alexey.tereshenkov  (1000) alexey.tereshenkov  (1000)     1836 2023-07-03 15:20:22.000000 pants-plugin-dep-graph-1.0.3/setup.py
```

### Comparing `pants-plugin-dep-graph-1.0.2/backend_shim.py` & `pants-plugin-dep-graph-1.0.3/backend_shim.py`

 * *Files identical despite different names*

### Comparing `pants-plugin-dep-graph-1.0.2/depgraph/backend/goal.py` & `pants-plugin-dep-graph-1.0.3/depgraph/backend/goal.py`

 * *Files identical despite different names*

### Comparing `pants-plugin-dep-graph-1.0.2/depgraph/backend/rules.py` & `pants-plugin-dep-graph-1.0.3/depgraph/backend/rules.py`

 * *Files identical despite different names*

### Comparing `pants-plugin-dep-graph-1.0.2/depgraph/backend/structs.py` & `pants-plugin-dep-graph-1.0.3/depgraph/backend/structs.py`

 * *Files identical despite different names*

### Comparing `pants-plugin-dep-graph-1.0.2/pants_plugin_dep_graph.egg-info/SOURCES.txt` & `pants-plugin-dep-graph-1.0.3/pants_plugin_dep_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pants-plugin-dep-graph-1.0.2/setup.py` & `pants-plugin-dep-graph-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # DO NOT EDIT THIS FILE -- AUTOGENERATED BY PANTS
-# Target: //:dist
+# Target: //:depgraph-plugin
 
 from setuptools import setup
 
 setup(**{
     'description': 'Pants plugin to export repository dependency graph.',
     'entry_points': {
         'pantsbuild.plugin': [
@@ -15,14 +15,21 @@
     'install_requires': (
         'pantsbuild.pants<2.17,>=2.16.0a0',
     ),
     'long_description': """# pants-dep-graph
 
 Pants plugin to query and export repository dependency graph. 
 
+Enable the plugin in your Pants repository:
+
+```
+[GLOBAL]
+plugins = ["pants-plugin-dep-graph==<release-version>"]
+```
+
 ## Examples
 
 ### Export dependencies 
 
 ```
 # only for Python sources
 pants dep-graph --filter-target-type=python_sources --deps src::
@@ -46,21 +53,36 @@
 
 ## Debugging
 
 ```
 pants --print-stacktrace --no-local-cache --no-pantsd dep-graph --deps src::
 pants --print-stacktrace --no-local-cache --no-pantsd dep-graph --rdeps src::
 ```
+
+## Analytics
+
+### Install
+
+```
+$ pip install dep-graph-analytics
+```
+
+### Usage
+
+```
+$ dep-graph-analytics cycles tests/cycles.json
+['src/moduleC.py', 'src/moduleA.py', 'src/moduleB.py']
+```
 """,
     'long_description_content_type': 'text/markdown',
     'name': 'pants-plugin-dep-graph',
     'namespace_packages': (
     ),
     'package_data': {
     },
     'packages': (
         'depgraph',
         'depgraph.backend',
     ),
     'python_requires': '>=3.9',
-    'version': '1.0.2',
+    'version': '1.0.3',
 })
```

