# Comparing `tmp/netbone-0.2.1.1.tar.gz` & `tmp/netbone-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbone-0.2.1.1.tar", last modified: Tue May 23 13:09:23 2023, max compression
+gzip compressed data, was "netbone-0.2.2.tar", last modified: Mon Jul  3 10:27:35 2023, max compression
```

## Comparing `netbone-0.2.1.1.tar` & `netbone-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,62 @@
-drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-23 13:09:23.594751 netbone-0.2.1.1/
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2803 2023-05-23 13:09:23.593751 netbone-0.2.1.1/PKG-INFO
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2534 2023-05-23 10:25:24.000000 netbone-0.2.1.1/README.md
-drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-23 13:09:23.186860 netbone-0.2.1.1/netbone/
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1637 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/__init__.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2549 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/backbone.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     4741 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/compare.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2938 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/filters.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1742 2023-05-07 00:59:21.000000 netbone-0.2.1.1/netbone/measures.py
-drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-23 13:09:23.289672 netbone-0.2.1.1/netbone/statistical/
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-02-26 17:47:23.000000 netbone-0.2.1.1/netbone/statistical/__init__.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1938 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/statistical/disparity.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1178 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/statistical/global_threshold.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)      990 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/statistical/lans.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)    11972 2023-05-07 00:22:39.000000 netbone-0.2.1.1/netbone/statistical/marginal_likelihood.py
-drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-23 13:09:23.357622 netbone-0.2.1.1/netbone/statistical/maxent_graph/
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     6232 2023-02-26 17:15:18.000000 netbone-0.2.1.1/netbone/statistical/maxent_graph/MaxentGraph.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)      279 2023-02-26 17:15:18.000000 netbone-0.2.1.1/netbone/statistical/maxent_graph/__init__.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     5713 2023-02-26 17:15:18.000000 netbone-0.2.1.1/netbone/statistical/maxent_graph/ecm.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1417 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/statistical/maxent_graph/ecm_main.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     3027 2023-05-07 00:22:39.000000 netbone-0.2.1.1/netbone/statistical/maxent_graph/util.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2058 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/statistical/noise_corrected.py
-drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-23 13:09:23.455482 netbone-0.2.1.1/netbone/structural/
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-03-19 17:00:02.000000 netbone-0.2.1.1/netbone/structural/__init__.py
-drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-23 13:09:23.535630 netbone-0.2.1.1/netbone/structural/distanceclosure/
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-02-26 17:15:18.000000 netbone-0.2.1.1/netbone/structural/distanceclosure/__init__.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     8491 2023-05-07 00:22:39.000000 netbone-0.2.1.1/netbone/structural/distanceclosure/backbone.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     7934 2023-05-06 23:26:37.000000 netbone-0.2.1.1/netbone/structural/distanceclosure/closure.py
-drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-23 13:09:23.549655 netbone-0.2.1.1/netbone/structural/distanceclosure/cython/
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-02-26 17:15:18.000000 netbone-0.2.1.1/netbone/structural/distanceclosure/cython/__init__.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     5043 2023-02-26 17:15:18.000000 netbone-0.2.1.1/netbone/structural/distanceclosure/dijkstra.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     8221 2023-02-26 17:15:18.000000 netbone-0.2.1.1/netbone/structural/distanceclosure/distance.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     5205 2023-02-26 17:15:18.000000 netbone-0.2.1.1/netbone/structural/distanceclosure/utils.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     3421 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/structural/doubly_stochastic.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2318 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/structural/h_backbone.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2136 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/structural/high_salience_skeleton.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1145 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/structural/maximum_spanning_tree.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2530 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/structural/metric_distance_backbone.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     7812 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/structural/modulairy_backbone.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2587 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/structural/ultrametric_distance_backbone.py
-drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-23 13:09:23.581715 netbone-0.2.1.1/netbone/utils/
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-07 03:39:24.000000 netbone-0.2.1.1/netbone/utils/__init__.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-07 03:39:24.000000 netbone-0.2.1.1/netbone/utils/narrate.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)      591 2023-05-23 10:19:05.000000 netbone-0.2.1.1/netbone/utils/utils.py
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)    10944 2023-05-09 01:06:55.000000 netbone-0.2.1.1/netbone/visualize.py
-drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-23 13:09:23.228366 netbone-0.2.1.1/netbone.egg-info/
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2803 2023-05-23 13:09:22.000000 netbone-0.2.1.1/netbone.egg-info/PKG-INFO
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1464 2023-05-23 13:09:23.000000 netbone-0.2.1.1/netbone.egg-info/SOURCES.txt
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)        1 2023-05-23 13:09:22.000000 netbone-0.2.1.1/netbone.egg-info/dependency_links.txt
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)      397 2023-05-23 13:09:22.000000 netbone-0.2.1.1/netbone.egg-info/requires.txt
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)        8 2023-05-23 13:09:22.000000 netbone-0.2.1.1/netbone.egg-info/top_level.txt
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)       38 2023-05-23 13:09:23.595750 netbone-0.2.1.1/setup.cfg
--rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1385 2023-05-23 13:09:20.000000 netbone-0.2.1.1/setup.py
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:35.277434 netbone-0.2.2/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2858 2023-07-03 10:27:35.277434 netbone-0.2.2/PKG-INFO
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2592 2023-07-03 10:00:00.000000 netbone-0.2.2/README.md
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:34.612444 netbone-0.2.2/netbone/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2125 2023-07-03 10:16:03.000000 netbone-0.2.2/netbone/__init__.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2338 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/backbone.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)    11044 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/compare.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     3125 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/filters.py
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:34.691294 netbone-0.2.2/netbone/hybrid/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/hybrid/__init__.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2086 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/hybrid/glanb.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1775 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/measures.py
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:34.773507 netbone-0.2.2/netbone/statistical/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-02-26 17:47:23.000000 netbone-0.2.2/netbone/statistical/__init__.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1258 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/statistical/disparity.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1034 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/statistical/lans.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)    11972 2023-05-07 00:22:39.000000 netbone-0.2.2/netbone/statistical/marginal_likelihood.py
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:34.868110 netbone-0.2.2/netbone/statistical/maxent_graph/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     6232 2023-02-26 17:15:18.000000 netbone-0.2.2/netbone/statistical/maxent_graph/MaxentGraph.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)      279 2023-02-26 17:15:18.000000 netbone-0.2.2/netbone/statistical/maxent_graph/__init__.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     5713 2023-02-26 17:15:18.000000 netbone-0.2.2/netbone/statistical/maxent_graph/ecm.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1461 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/statistical/maxent_graph/ecm_main.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     3027 2023-05-07 00:22:39.000000 netbone-0.2.2/netbone/statistical/maxent_graph/util.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2102 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/statistical/noise_corrected.py
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:35.088450 netbone-0.2.2/netbone/structural/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-03-19 17:00:02.000000 netbone-0.2.2/netbone/structural/__init__.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1208 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/betweenness.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1045 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/degree.py
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:35.214164 netbone-0.2.2/netbone/structural/distanceclosure/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-02-26 17:15:18.000000 netbone-0.2.2/netbone/structural/distanceclosure/__init__.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     8491 2023-05-07 00:22:39.000000 netbone-0.2.2/netbone/structural/distanceclosure/backbone.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     7934 2023-05-06 23:26:37.000000 netbone-0.2.2/netbone/structural/distanceclosure/closure.py
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:35.229776 netbone-0.2.2/netbone/structural/distanceclosure/cython/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-02-26 17:15:18.000000 netbone-0.2.2/netbone/structural/distanceclosure/cython/__init__.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     5043 2023-02-26 17:15:18.000000 netbone-0.2.2/netbone/structural/distanceclosure/dijkstra.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     8221 2023-02-26 17:15:18.000000 netbone-0.2.2/netbone/structural/distanceclosure/distance.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     5205 2023-02-26 17:15:18.000000 netbone-0.2.2/netbone/structural/distanceclosure/utils.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     3505 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/doubly_stochastic.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)      725 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/global_threshold.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1048 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/gspar.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2128 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/h_backbone.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1937 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/high_salience_skeleton.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)      969 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/maximum_spanning_tree.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)      923 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/metric_distance_backbone.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2709 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/mlam.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2704 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/modulairy_backbone.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1203 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/plam.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1194 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/pmfg.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)      940 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/structural/ultrametric_distance_backbone.py
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:35.264930 netbone-0.2.2/netbone/utils/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-07 03:39:24.000000 netbone-0.2.2/netbone/utils/__init__.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-05-07 03:39:24.000000 netbone-0.2.2/netbone/utils/narrate.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)      598 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/utils/utils.py
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)    10927 2023-07-03 09:53:38.000000 netbone-0.2.2/netbone/visualize.py
+drwxrwxrwx   0 yassin    (1000) yassin    (1000)        0 2023-07-03 10:27:34.667646 netbone-0.2.2/netbone.egg-info/
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     2858 2023-07-03 10:27:34.000000 netbone-0.2.2/netbone.egg-info/PKG-INFO
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1686 2023-07-03 10:27:34.000000 netbone-0.2.2/netbone.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)        1 2023-07-03 10:27:34.000000 netbone-0.2.2/netbone.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)      397 2023-07-03 10:27:34.000000 netbone-0.2.2/netbone.egg-info/requires.txt
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)        8 2023-07-03 10:27:34.000000 netbone-0.2.2/netbone.egg-info/top_level.txt
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)       38 2023-07-03 10:27:35.277434 netbone-0.2.2/setup.cfg
+-rwxrwxrwx   0 yassin    (1000) yassin    (1000)     1383 2023-07-03 10:06:36.000000 netbone-0.2.2/setup.py
```

### Comparing `netbone-0.2.1.1/PKG-INFO` & `netbone-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbone
-Version: 0.2.1.1
+Version: 0.2.2
 Summary: A python package for extracting network backbones from simple weighted networks
 Home-page: https://gitlab.liris.cnrs.fr/coregraphie/netbone
 Author: Ali Yassin
 Author-email: aliyassin4@hotmail.com
 License: MIT
 Keywords: backbone network
 Description-Content-Type: text/markdown
@@ -14,15 +14,16 @@
 
 NetBone is a Python library for extracting network backbones from simple weighted networks.
 
 ## Features
 
 - Extract network backbones from simple weighted networks
 - Contains six statistical methods for extracting backbones
-- Contains seven structural methods for extracting backbones
+- Contains thirteen structural methods for extracting backbones
+- Contains one hybrid method for extracting backbones
 - Includes three filters for extracting the backbone: boolean filter, threshold filter, and fraction filter
 - Built-in methods for comparing backbones with each other
 - Option to use custom comparison methods
 - Visualization tools to display the results of the comparison
```

### Comparing `netbone-0.2.1.1/README.md` & `netbone-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 NetBone is a Python library for extracting network backbones from simple weighted networks.
 
 ## Features
 
 - Extract network backbones from simple weighted networks
 - Contains six statistical methods for extracting backbones
-- Contains seven structural methods for extracting backbones
+- Contains thirteen structural methods for extracting backbones
+- Contains one hybrid method for extracting backbones
 - Includes three filters for extracting the backbone: boolean filter, threshold filter, and fraction filter
 - Built-in methods for comparing backbones with each other
 - Option to use custom comparison methods
 - Visualization tools to display the results of the comparison
```

### Comparing `netbone-0.2.1.1/netbone/__init__.py` & `netbone-0.2.2/netbone/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,32 +12,42 @@
 from netbone.statistical.noise_corrected import noise_corrected
 from netbone.structural.doubly_stochastic import doubly_stochastic
 from netbone.structural.high_salience_skeleton import high_salience_skeleton
 from netbone.statistical.marginal_likelihood import MLF
 from netbone.statistical.lans import lans
 from netbone.structural.ultrametric_distance_backbone import ultrametric_distance_backbone
 from netbone.structural.metric_distance_backbone import metric_distance_backbone
-from netbone.statistical.global_threshold import global_threshold
+from netbone.structural.global_threshold import global_threshold
 from netbone.structural.modulairy_backbone import modularity_backbone
 from netbone.structural.maximum_spanning_tree import maximum_spanning_tree
+from netbone.hybrid.glanb import glanb
+from netbone.structural.pmfg import pmfg
+from netbone.structural.plam import plam
+from netbone.structural.mlam import mlam
+from netbone.structural.gspar import gspar
+from netbone.structural.degree import degree
+from netbone.structural.betweenness import betweenness
+# from netbone.structural.mad import mad
+# # from netbone.statistical.correlation_and_statistic import correlation_and_statistic
+
 from netbone.filters import threshold_filter, fraction_filter
 from netbone import compare
 from netbone import filters
 from netbone import visualize
 from netbone.backbone import Backbone
 try:
     from netbone.statistical.maxent_graph.ecm_main import ecm
 except ImportError:
     print("Can't load ECM Model in windows, try using it on linux")
 
 
 def marginal_likelihood(data):
     data = data.copy()
     mlf = MLF(directed=False)
-    return Backbone(mlf.fit_transform(data), name="Marginal Likelihood Filter", column="p_value", ascending=True, filters=[threshold_filter, fraction_filter])
+    return Backbone(mlf.fit_transform(data), method_name="Marginal Likelihood Filter", property_name="p_value", ascending=True, compatible_filters=[threshold_filter, fraction_filter], filter_on='Edges')
 
 
 
 
 # logger = logging.getLogger()
 # logger.setLevel('DEBUG')
```

### Comparing `netbone-0.2.1.1/netbone/filters.py` & `netbone-0.2.2/netbone/filters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,77 @@
 import math
 
 import networkx as nx
 from netbone.utils.utils import edge_properties
+
+
 def boolean_filter(backbone, narrate=True, value=[]):
-    if boolean_filter in backbone.filters():
+    if boolean_filter in backbone.compatible_filters():
         data = backbone.graph
-        column = backbone.column
+        column = 'in_backbone'
         if isinstance(data, nx.Graph):
             data = nx.to_pandas_edgelist(data)
         if narrate:
             backbone.narrate()
-        return nx.from_pandas_edgelist(data[data[column] == True], edge_attr=edge_properties(data))
-    print("The accepted filters for " + backbone.name + " are: " + ', '.join([fun.__name__ for fun in backbone.filters()]))
-
-def threshold_filter(backbone, value, narrate=True , secondary_column = 'weight', secondary_column_ascending = False, **kwargs):
-    data = backbone.graph
-    column = backbone.column
-    ascending = backbone.ascending
-
-    if isinstance(data, nx.Graph):
-        data = nx.to_pandas_edgelist(data)
-
-    keys = kwargs.keys()
-    if "value" in keys:
-        value = kwargs["value"]
-    if "secondary_column" in keys:
-        secondary_column = kwargs['secondary_column']
-
-    if threshold_filter in backbone.filters():
-        if boolean_filter in backbone.filters():
-            column = 'score'
-        data = data.sort_values(by=[column, secondary_column], ascending=[ascending, secondary_column_ascending])
+        return nx.from_pandas_edgelist(data[data[column]], edge_attr=edge_properties(data))
+    print("The accepted filters for " + backbone.method_name + " are: " + ', '.join(
+        [fun.__name__ for fun in backbone.compatible_filters()]))
+
+
+def threshold_filter(backbone, value, narrate=True, secondary_property='weight', secondary_property_ascending=False,
+                     **kwargs):
+    data = backbone.to_dataframe()
+    property_name = backbone.property_name
+    filter_by = [property_name]
+    ascending = [backbone.ascending]
+
+    if backbone.filter_on == 'Edges':
+        filter_by.append(secondary_property)
+        ascending.append(secondary_property_ascending)
+
+    if threshold_filter in backbone.compatible_filters():
+        data = data.sort_values(by=filter_by,
+                                ascending=ascending)
 
         if narrate:
             backbone.narrate()
 
-        if column == "p_value":
-            return nx.from_pandas_edgelist(data[data[column] < value], edge_attr=edge_properties(data))
-        elif column == "score":
-            return nx.from_pandas_edgelist(data[data[column] > value], edge_attr=edge_properties(data))
+        if backbone.ascending:
+            data = data[data[property_name] < value]
+            if backbone.filter_on == 'Edges':
+                return nx.from_pandas_edgelist(data, edge_attr=edge_properties(data))
+            return backbone.graph.subgraph(list(data.index)).copy()
         else:
-            print("Column name can not be " + column)
-
-    print("The accepted filters for " + backbone.name + " are: " + ', '.join([fun.__name__ for fun in backbone.filters()]))
-
-
-
+            data = data[data[property_name] > value]
+            if backbone.filter_on == 'Edges':
+                return nx.from_pandas_edgelist(data, edge_attr=edge_properties(data))
+            return backbone.graph.subgraph(list(data.index)).copy()
+
+    print("The accepted filters for " + backbone.method_name + " are: " + ', '.join(
+        [fun.__name__ for fun in backbone.compatible_filters()]))
+
+
+def fraction_filter(backbone, value, narrate=True, secondary_property='weight', secondary_property_ascending=False,
+                    **kwargs):
+    data = backbone.to_dataframe()
+    filter_by = [backbone.property_name]
+    ascending = [backbone.ascending]
+
+    if backbone.filter_on == 'Edges':
+        filter_by.append(secondary_property)
+        ascending.append(secondary_property_ascending)
 
-def fraction_filter(backbone, value, narrate=True, secondary_column='weight', secondary_column_ascending=False, **kwargs):
-    data = backbone.graph
-    column = backbone.column
-    ascending = backbone.ascending
-
-    if isinstance(data, nx.Graph):
-        data = nx.to_pandas_edgelist(data)
-
-    keys = kwargs.keys()
-    if "value" in keys:
-        value = kwargs["value"]
-    if "secondary_column" in keys:
-        secondary_column = kwargs['secondary_column']
-
-    value = math.ceil(value * len(data))
-
-    if fraction_filter in backbone.filters():
-        if boolean_filter in backbone.filters():
-            column = 'score'
-        data = data.sort_values(by=[column, secondary_column], ascending=[ascending, secondary_column_ascending])
+    if fraction_filter in backbone.compatible_filters():
+        data = data.sort_values(by=filter_by, ascending=ascending)
 
         if narrate:
             backbone.narrate()
-        return nx.from_pandas_edgelist(data[:value], edge_attr=edge_properties(data))
-
-    print("The accepted filters for " + backbone.name + " are: " + ', '.join([fun.__name__ for fun in backbone.filters()]))
-
-    
-    
 
+        if backbone.filter_on == 'Edges':
+            value = math.ceil(value * len(data))
+            return nx.from_pandas_edgelist(data[:value], edge_attr=edge_properties(data))
+        else:
+            value = math.ceil(value * len(backbone.graph))
+            return backbone.graph.subgraph(list(data[:value].index)).copy()
 
+    print("The accepted filters for " + backbone.method_name + " are: " + ', '.join(
+        [fun.__name__ for fun in backbone.compatible_filters()]))
```

### Comparing `netbone-0.2.1.1/netbone/measures.py` & `netbone-0.2.2/netbone/measures.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def reachability(original, G):
     r = 0
     for c in [len(component) for component in nx.connected_components(G)]:
         r += c*(c-1)
     return r/(len(G)*(len(G) - 1))
 
 def number_connected_components(original, G):
-    nx.number_connected_components(G)
+    return nx.number_connected_components(G)
 
 def diameter(original, G):
     return ig.Graph.from_networkx(lcc(G)).diameter(directed=False, unconn=True)
 
 def lcc_node_fraction(G):
     return node_fraction(G, lcc(G))
 
@@ -49,16 +49,16 @@
 
 def lcc_weight_fraction(original, G):
     return weight_fraction(G, lcc(G))
 
 def weights(G):
     return list(nx.get_edge_attributes(G, 'weight').values())
 
-def degrees(G):
-    return list(dict(G.degree()).values())
+def degrees(G, weight=None):
+    return list(dict(G.degree(weight=weight)).values())
 
 def average_clustering_coefficient(original, G):
     node_clustering = ig.Graph.from_networkx(G).transitivity_local_undirected(mode="nan")
     return np.mean([x for x in node_clustering if isinstance(x, float) and not np.isnan(x)])
 
 def transitivity(original, graph):
     return nx.transitivity(graph)
```

### Comparing `netbone-0.2.1.1/netbone/statistical/disparity.py` & `netbone-0.2.2/netbone/statistical/disparity.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,25 +24,8 @@
                 p_ij = w/strength[node]
                 alpha_ij = (1-p_ij)**(k-1)
                 if 'p_value' in g[node][neighbour]:
                     if alpha_ij < g[node][neighbour]['p_value']:
                         g[node][neighbour]['p_value'] = alpha_ij
                 else:
                     g[node][neighbour]['p_value'] = alpha_ij
-    return Backbone(g, name="Disparity Filter", column="p_value", ascending=True, filters=[threshold_filter, fraction_filter])
-
-    # b = nx.Graph()
-    # for u in g:
-    #     k = len(g[u])
-    #     if k > 1:
-    #         sum_w = sum(np.absolute(g[u][v][weight]) for v in g[u])
-    #         for v in g[u]:
-    #             w = g[u][v][weight]
-    #             p_ij = float(np.absolute(w))/sum_w
-    #             alpha_ij = 1 - \
-    #                        (k-1) * integrate.quad(lambda x: (1-x)
-    #                                                         ** (k-2), 0, p_ij)[0]
-    #             # float('%.4f' % alpha_ij)
-    #             b.add_edge(u, v, weight=w, p_value=float(alpha_ij))
-    # return Backbone(b, name="Disparity Filter", column="p_value", ascending=True, filters=[threshold_filter, fraction_filter])
-
-
+    return Backbone(g, method_name="Disparity Filter", property_name="p_value", ascending=True, compatible_filters=[threshold_filter, fraction_filter], filter_on='Edges')
```

### Comparing `netbone-0.2.1.1/netbone/statistical/global_threshold.py` & `netbone-0.2.2/netbone/structural/global_threshold.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,15 @@
 from networkx import Graph,to_pandas_edgelist
 from netbone.utils.utils import edge_properties
 from netbone.backbone import Backbone
 from netbone.filters import fraction_filter, threshold_filter
 def global_threshold(data):
 
     if isinstance(data, DataFrame):
-        table = data.copy()
+        g = nx.from_pandas_edgelist(data, edge_attr=edge_properties(data))
     elif isinstance(data, Graph):
-        table = to_pandas_edgelist(data)
-        is_graph=True
+        g = data.copy()
     else:
         print("data should be a panads dataframe or nx graph")
         return
 
-    table['score'] = table['weight']
-
-    g = nx.from_pandas_edgelist(table, edge_attr=edge_properties(table))
-    # average = table['weight'].mean()
-    # for u,v in g.edges():
-    #     if g[u][v]['score']>=average:
-    #         g[u][v]['global_threshold'] = True
-    #     else:
-    #         g[u][v]['global_threshold'] = False
-    # return Backbone(g, name="Global Threshold Filter", column="global_threshold", ascending=False, filters=[boolean_filter, fraction_filter, threshold_filter])
-    return Backbone(g, name="Global Threshold Filter", column="score", ascending=False, filters=[fraction_filter, threshold_filter])
+    return Backbone(g, method_name="Global Threshold Filter", property_name="weight", ascending=False, compatible_filters=[fraction_filter, threshold_filter], filter_on='Edges')
```

### Comparing `netbone-0.2.1.1/netbone/statistical/lans.py` & `netbone-0.2.2/netbone/statistical/lans.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     elif isinstance(data, nx.Graph):
         g = data.copy()
     else:
         print("data should be a panads dataframe or nx graph")
         return
     for u, v, w in g.edges(data='weight'):
         g[u][v]['p_value'] = min(compute_pvalue(g, v, w), compute_pvalue(g, u, w))
-    return Backbone(g, name="Locally Adaptive Network Sparsification Filter", column="p_value", ascending=True,
-                    filters=[threshold_filter, fraction_filter])
+    return Backbone(g, method_name="Locally Adaptive Network Sparsification Filter", property_name="p_value", ascending=True,
+                    compatible_filters=[threshold_filter, fraction_filter], filter_on='Edges')
 
 
 def compute_pvalue(G, node, w):
     u_degree = G.degree(node, weight='weight')
     puv = w / u_degree
     u_n = G[node]
     count = len([n for n in u_n if u_n[n]['weight'] / u_degree <= puv])
```

### Comparing `netbone-0.2.1.1/netbone/statistical/marginal_likelihood.py` & `netbone-0.2.2/netbone/statistical/marginal_likelihood.py`

 * *Files identical despite different names*

### Comparing `netbone-0.2.1.1/netbone/statistical/maxent_graph/MaxentGraph.py` & `netbone-0.2.2/netbone/statistical/maxent_graph/MaxentGraph.py`

 * *Files identical despite different names*

### Comparing `netbone-0.2.1.1/netbone/statistical/maxent_graph/ecm.py` & `netbone-0.2.2/netbone/statistical/maxent_graph/ecm.py`

 * *Files identical despite different names*

### Comparing `netbone-0.2.1.1/netbone/statistical/maxent_graph/ecm_main.py` & `netbone-0.2.2/netbone/statistical/maxent_graph/ecm_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     # def filter_edge(n1, n2):
     #     return g[n1][n2]['p_value'] > -np.log(0.10)
     
     g = nx.relabel_nodes(g, dict(zip(g.nodes(), data.nodes())))
 
     nx.set_edge_attributes(data, {(u,v):w for u,v,w in list(g.edges(data='p_value'))}, name='p_value')
     #subgraph = nx.subgraph_view(g)#, filter_edge=filter_edge)
-    return Backbone(data, name="Enhanced Configuration Model Filter", column="p_value", ascending=True, filters=[threshold_filter, fraction_filter])
+    return Backbone(data, method_name="Enhanced Configuration Model Filter", property_name="p_value", ascending=True, compatible_filters=[threshold_filter, fraction_filter], filter_on='Edges')
```

### Comparing `netbone-0.2.1.1/netbone/statistical/maxent_graph/util.py` & `netbone-0.2.2/netbone/statistical/maxent_graph/util.py`

 * *Files identical despite different names*

### Comparing `netbone-0.2.1.1/netbone/statistical/noise_corrected.py` & `netbone-0.2.2/netbone/statistical/noise_corrected.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,9 +36,9 @@
             variance_nij = expected_pij * (1 - expected_pij) * n
             d = (1.0 / (ni * nj)) - (n * ((ni + nj) / ((ni * nj) ** 2)))
             variance_cij = variance_nij * (((2 * (kappa + (w * d))) / (((kappa * w) + 1) ** 2)) ** 2)
             sdev_cij = variance_cij ** .5
             g[i][j]['nc_sdev'] = sdev_cij
             g[i][j]['score'] = score
 
-    return Backbone(g, name="Noise Corrected Filter", column="p_value", ascending=True, filters=[threshold_filter, fraction_filter])
+    return Backbone(g, method_name="Noise Corrected Filter", property_name="p_value", ascending=True, compatible_filters=[threshold_filter, fraction_filter], filter_on='Edges')
```

### Comparing `netbone-0.2.1.1/netbone/structural/distanceclosure/backbone.py` & `netbone-0.2.2/netbone/structural/distanceclosure/backbone.py`

 * *Files identical despite different names*

### Comparing `netbone-0.2.1.1/netbone/structural/distanceclosure/closure.py` & `netbone-0.2.2/netbone/structural/distanceclosure/closure.py`

 * *Files identical despite different names*

### Comparing `netbone-0.2.1.1/netbone/structural/distanceclosure/dijkstra.py` & `netbone-0.2.2/netbone/structural/distanceclosure/dijkstra.py`

 * *Files identical despite different names*

### Comparing `netbone-0.2.1.1/netbone/structural/distanceclosure/distance.py` & `netbone-0.2.2/netbone/structural/distanceclosure/distance.py`

 * *Files identical despite different names*

### Comparing `netbone-0.2.1.1/netbone/structural/distanceclosure/utils.py` & `netbone-0.2.2/netbone/structural/distanceclosure/utils.py`

 * *Files identical despite different names*

### Comparing `netbone-0.2.1.1/netbone/structural/doubly_stochastic.py` & `netbone-0.2.2/netbone/structural/doubly_stochastic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import warnings
 import numpy as np
 import pandas as pd
 import networkx as nx
 from netbone.backbone import Backbone
 from netbone.filters import boolean_filter, threshold_filter, fraction_filter
+
 # algo: doubly_stochastic.py
 warnings.filterwarnings('ignore')
 
+
 def doubly_stochastic(data):
-    
-    undirected=True
-    return_self_loops=False
+    undirected = True
+    return_self_loops = False
 
     if isinstance(data, pd.DataFrame):
         table = data.copy()
     elif isinstance(data, nx.Graph):
         table = nx.to_pandas_edgelist(data)
     else:
         print("data should be a panads dataframe or nx graph")
@@ -36,43 +37,45 @@
             warnings.warn(
                 "Matrix could not be reduced to doubly stochastic. See Sec. 3 of Sinkhorn 1964", RuntimeWarning)
             return pd.DataFrame()
     table = pd.melt(table.reset_index(), id_vars="source")
     table = table[table["source"] < table["target"]]
     table = table[table["value"] > 0].sort_values(by="value", ascending=False)
     table = table.merge(table2[["source", "target", "weight"]], on=[
-                        "source", "target"])
+        "source", "target"])
     i = 0
     doubly_nodes = len(set(table["source"]) | set(table["target"]))
     edges = table.shape[0]
     if undirected:
         G = nx.Graph()
         while nx.number_connected_components(G) != 1 or len(G) < doubly_nodes or nx.is_connected(G) == False:
             if i == edges:
                 break
             edge = table.iloc[i]
             G.add_edge(edge["source"], edge["target"], weight=edge["value"])
             table.loc[table.loc[(table['source'] == edge["source"]) & (
-                table['target'] == edge["target"])].index[0], 'ds_backbone'] = True
+                    table['target'] == edge["target"])].index[0], 'in_backbone'] = True
             i += 1
     else:
         G = nx.DiGraph()
         while nx.number_weakly_connected_components(G) != 1 or len(G) < doubly_nodes or nx.is_connected(G) == False:
-            if i== edges:
+            if i == edges:
                 break
             edge = table.iloc[i]
             G.add_edge(edge["source"], edge["target"], weight=edge["value"])
             table.loc[table.loc[(table['source'] == edge["source"]) & (
-                table['target'] == edge["target"])].index[0], 'ds_backbone'] = True
+                    table['target'] == edge["target"])].index[0], 'in_backbone'] = True
             i += 1
 
     # table = pd.melt(nx.to_pandas_adjacency(G).reset_index(), id_vars = "index")
     table = table[table["value"] >= 0]
     table.rename(columns={"index": "source",
-                 "variable": "target", "value": "score"}, inplace=True)
+                          "variable": "target", "value": "score"}, inplace=True)
     table = table.fillna(False)
     if not return_self_loops:
         table = table[table["source"] != table["target"]]
     if undirected:
         table = table[table["source"] <= table["target"]]
 
-    return Backbone(nx.from_pandas_edgelist(table, edge_attr=['weight', 'score', 'ds_backbone']), name="Doubly Stochastic Filter", column="ds_backbone", ascending=False, filters=[boolean_filter, threshold_filter, fraction_filter])
+    return Backbone(nx.from_pandas_edgelist(table, edge_attr=['weight', 'score', 'in_backbone']),
+                    method_name="Doubly Stochastic Filter", property_name="score", ascending=False,
+                    compatible_filters=[boolean_filter, threshold_filter, fraction_filter], filter_on='Edges')
```

### Comparing `netbone-0.2.1.1/netbone/structural/h_backbone.py` & `netbone-0.2.2/netbone/structural/h_backbone.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import networkx as nx
 import pandas as pd
 from netbone.backbone import Backbone
 from netbone.filters import boolean_filter
+
+
 # algo: h_backbone
 # calculating H-Index
 
 def h_backbone(data):
-    is_graph=False
-
     if isinstance(data, pd.DataFrame):
         G = nx.from_pandas_edgelist(data, edge_attr='weight', create_using=nx.Graph())
     elif isinstance(data, nx.Graph):
         G = data.copy()
-        is_graph=True
     else:
         print("data should be a panads dataframe or nx graph")
         return
 
     betweenness_values = nx.edge_betweenness_centrality(
         G, weight='weight', normalized=False)
 
     nx.set_edge_attributes(G, {edge: {'h_bridge': round(
-        betweenness_values[edge]/len(G.nodes()), 3)} for edge in betweenness_values})
-#     for u, v in G.edges():
-#         G[u][v]['bridge'] = round(betweenness_values[(u,v)]/len(G.nodes()),3)
+        betweenness_values[edge] / len(G.nodes()), 3)} for edge in betweenness_values})
+    #     for u, v in G.edges():
+    #         G[u][v]['bridge'] = round(betweenness_values[(u,v)]/len(G.nodes()),3)
 
     weight_values = list(nx.get_edge_attributes(G, 'weight').values())
     bridge_values = list(nx.get_edge_attributes(G, 'h_bridge').values())
 
     # sorting in ascending order
     weight_values.sort()
     bridge_values.sort()
@@ -55,14 +54,13 @@
         # if result is less than or equal
         # to cited then return result
         if h_bridge <= cited:
             break
 
     for u, v in G.edges():
         if G[u][v]['h_bridge'] >= h_bridge or G[u][v]['weight'] >= h_weight:
-            G[u][v]['h_backbone'] = True
+            G[u][v]['in_backbone'] = True
         else:
-            G[u][v]['h_backbone'] = False
-    if is_graph:
-        return Backbone(G, name="H-Backbone Filter", column="h_backbone", ascending=False, filters=[boolean_filter]) #h_bridge, h_weight, G
-    # return nx.to_pandas_edgelist(G.to_directed()), "h_backbone"
-    return Backbone(nx.to_pandas_edgelist(G), name="H-Backbone Filter", column="h_backbone", ascending=False, filters=[boolean_filter])
+            G[u][v]['in_backbone'] = False
+
+    return Backbone(nx.to_pandas_edgelist(G), method_name="H-Backbone Filter", property_name="h_bridge",
+                    ascending=False, compatible_filters=[boolean_filter], filter_on='Edges')
```

### Comparing `netbone-0.2.1.1/netbone/structural/high_salience_skeleton.py` & `netbone-0.2.2/netbone/structural/high_salience_skeleton.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,122 @@
-00000000: 0d0a 6672 6f6d 2063 6f6c 6c65 6374 696f  ..from collectio
-00000010: 6e73 2069 6d70 6f72 7420 6465 6661 756c  ns import defaul
-00000020: 7464 6963 740d 0a69 6d70 6f72 7420 6e65  tdict..import ne
-00000030: 7477 6f72 6b78 2061 7320 6e78 0d0a 696d  tworkx as nx..im
-00000040: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
-00000050: 640d 0a69 6d70 6f72 7420 7761 726e 696e  d..import warnin
-00000060: 6773 0d0a 6672 6f6d 206e 6574 626f 6e65  gs..from netbone
-00000070: 2e62 6163 6b62 6f6e 6520 696d 706f 7274  .backbone import
-00000080: 2042 6163 6b62 6f6e 650d 0a66 726f 6d20   Backbone..from 
-00000090: 6e65 7462 6f6e 652e 6669 6c74 6572 7320  netbone.filters 
-000000a0: 696d 706f 7274 2062 6f6f 6c65 616e 5f66  import boolean_f
-000000b0: 696c 7465 722c 2074 6872 6573 686f 6c64  ilter, threshold
-000000c0: 5f66 696c 7465 722c 2066 7261 6374 696f  _filter, fractio
-000000d0: 6e5f 6669 6c74 6572 0d0a 0d0a 2320 6368  n_filter....# ch
-000000e0: 616e 6765 2064 6973 7461 6e63 650d 0a64  ange distance..d
-000000f0: 6566 2068 6967 685f 7361 6c69 656e 6365  ef high_salience
-00000100: 5f73 6b65 6c65 746f 6e28 6461 7461 293a  _skeleton(data):
-00000110: 0d0a 2020 2020 6966 2069 7369 6e73 7461  ..    if isinsta
-00000120: 6e63 6528 6461 7461 2c20 7064 2e44 6174  nce(data, pd.Dat
-00000130: 6146 7261 6d65 293a 0d0a 2020 2020 2020  aFrame):..      
-00000140: 2020 6772 6170 6820 3d20 6e78 2e66 726f    graph = nx.fro
-00000150: 6d5f 7061 6e64 6173 5f65 6467 656c 6973  m_pandas_edgelis
-00000160: 7428 6461 7461 2c20 6564 6765 5f61 7474  t(data, edge_att
-00000170: 723d 2777 6569 6768 7427 2c20 6372 6561  r='weight', crea
-00000180: 7465 5f75 7369 6e67 3d6e 782e 4772 6170  te_using=nx.Grap
-00000190: 6828 2929 0d0a 2020 2020 656c 6966 2069  h())..    elif i
-000001a0: 7369 6e73 7461 6e63 6528 6461 7461 2c20  sinstance(data, 
-000001b0: 6e78 2e47 7261 7068 293a 0d0a 2020 2020  nx.Graph):..    
-000001c0: 2020 2020 6772 6170 6820 3d20 6461 7461      graph = data
-000001d0: 2e63 6f70 7928 290d 0a20 2020 2065 6c73  .copy()..    els
-000001e0: 653a 0d0a 2020 2020 2020 2020 7072 696e  e:..        prin
-000001f0: 7428 2264 6174 6120 7368 6f75 6c64 2062  t("data should b
-00000200: 6520 6120 7061 6e61 6473 2064 6174 6166  e a panads dataf
-00000210: 7261 6d65 206f 7220 6e78 2067 7261 7068  rame or nx graph
-00000220: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
-00000230: 726e 0d0a 0d0a 2020 2020 7765 733d 206e  rn....    wes= n
-00000240: 782e 6765 745f 6564 6765 5f61 7474 7269  x.get_edge_attri
-00000250: 6275 7465 7328 6772 6170 682c 2027 7765  butes(graph, 'we
-00000260: 6967 6874 2729 0d0a 2020 2020 7661 6c75  ight')..    valu
-00000270: 6573 203d 207b 7061 6972 3a31 2f77 6573  es = {pair:1/wes
-00000280: 5b70 6169 725d 2066 6f72 2070 6169 7220  [pair] for pair 
-00000290: 696e 2077 6573 7d0d 0a20 2020 206e 782e  in wes}..    nx.
-000002a0: 7365 745f 6564 6765 5f61 7474 7269 6275  set_edge_attribu
-000002b0: 7465 7328 6772 6170 682c 2076 616c 7565  tes(graph, value
-000002c0: 732c 206e 616d 653d 2764 6973 7461 6e63  s, name='distanc
-000002d0: 6527 290d 0a0d 0a20 2020 206e 782e 7365  e')....    nx.se
-000002e0: 745f 6564 6765 5f61 7474 7269 6275 7465  t_edge_attribute
-000002f0: 7328 6772 6170 682c 2030 2c20 6e61 6d65  s(graph, 0, name
-00000300: 3d27 7363 6f72 6527 290d 0a0d 0a20 2020  ='score')....   
-00000310: 2066 6f72 2073 6f75 7263 6520 696e 2067   for source in g
-00000320: 7261 7068 2e6e 6f64 6573 2829 3a0d 0a20  raph.nodes():.. 
-00000330: 2020 2020 2020 2074 7265 6520 3d20 6e78         tree = nx
-00000340: 2e73 696e 676c 655f 736f 7572 6365 5f64  .single_source_d
-00000350: 696a 6b73 7472 6128 6772 6170 682c 2073  ijkstra(graph, s
-00000360: 6f75 7263 652c 2063 7574 6f66 663d 4e6f  ource, cutoff=No
-00000370: 6e65 2c20 7765 6967 6874 3d27 6469 7374  ne, weight='dist
-00000380: 616e 6365 2729 5b31 5d0d 0a20 2020 2020  ance')[1]..     
-00000390: 2020 206e 6f64 655f 7472 6565 5f73 636f     node_tree_sco
-000003a0: 7265 7320 3d20 6469 6374 2829 0d0a 0d0a  res = dict()....
-000003b0: 2020 2020 2020 2020 7061 7468 7320 3d20          paths = 
-000003c0: 6c69 7374 2874 7265 652e 7661 6c75 6573  list(tree.values
-000003d0: 2829 295b 313a 5d0d 0a20 2020 2020 2020  ())[1:]..       
-000003e0: 2066 6f72 2070 6174 6820 696e 2070 6174   for path in pat
-000003f0: 6873 3a0d 0a20 2020 2020 2020 2020 2020  hs:..           
-00000400: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00000410: 6c65 6e28 7061 7468 2920 2d20 3129 3a0d  len(path) - 1):.
-00000420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000430: 206e 6f64 655f 7472 6565 5f73 636f 7265   node_tree_score
-00000440: 735b 2870 6174 685b 695d 2c20 7061 7468  s[(path[i], path
-00000450: 5b69 2b31 5d29 5d20 3d20 310d 0a0d 0a20  [i+1])] = 1.... 
-00000460: 2020 2020 2020 2066 6f72 2075 2c76 2069         for u,v i
-00000470: 6e20 6e6f 6465 5f74 7265 655f 7363 6f72  n node_tree_scor
-00000480: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-00000490: 2067 7261 7068 5b75 5d5b 765d 5b27 7363   graph[u][v]['sc
-000004a0: 6f72 6527 5d20 2b3d 310d 0a0d 0a20 2020  ore'] +=1....   
-000004b0: 2073 636f 7265 733d 206e 782e 6765 745f   scores= nx.get_
-000004c0: 6564 6765 5f61 7474 7269 6275 7465 7328  edge_attributes(
-000004d0: 6772 6170 682c 2027 7363 6f72 6527 290d  graph, 'score').
-000004e0: 0a20 2020 204e 203d 206c 656e 2867 7261  .    N = len(gra
-000004f0: 7068 290d 0a20 2020 2073 636f 7265 5f76  ph)..    score_v
-00000500: 616c 7565 7320 3d20 6469 6374 2829 0d0a  alues = dict()..
-00000510: 2020 2020 6261 636b 626f 6e65 5f65 6467      backbone_edg
-00000520: 6573 203d 2064 6963 7428 290d 0a20 2020  es = dict()..   
-00000530: 2066 6f72 2070 6169 7220 696e 2073 636f   for pair in sco
-00000540: 7265 733a 0d0a 2020 2020 2020 2020 7363  res:..        sc
-00000550: 6f72 655f 7661 6c75 6573 5b70 6169 725d  ore_values[pair]
-00000560: 203d 2073 636f 7265 735b 7061 6972 5d2f   = scores[pair]/
-00000570: 4e0d 0a20 2020 2020 2020 2069 6620 7363  N..        if sc
-00000580: 6f72 6573 5b70 6169 725d 2f4e 203e 2030  ores[pair]/N > 0
-00000590: 2e38 3a0d 0a20 2020 2020 2020 2020 2020  .8:..           
-000005a0: 2062 6163 6b62 6f6e 655f 6564 6765 735b   backbone_edges[
-000005b0: 7061 6972 5d20 3d20 5472 7565 0d0a 2020  pair] = True..  
-000005c0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-000005d0: 2020 2020 2020 2020 2062 6163 6b62 6f6e           backbon
-000005e0: 655f 6564 6765 735b 7061 6972 5d20 3d20  e_edges[pair] = 
-000005f0: 4661 6c73 650d 0a0d 0a20 2020 2020 2020  False....       
-00000600: 2020 2020 2023 2073 636f 7265 5f76 616c       # score_val
-00000610: 7565 7320 3d20 7b70 6169 723a 7363 6f72  ues = {pair:scor
-00000620: 6573 5b70 6169 725d 2f4e 2066 6f72 2070  es[pair]/N for p
-00000630: 6169 7220 696e 2073 636f 7265 737d 0d0a  air in scores}..
-00000640: 2020 2020 6e78 2e73 6574 5f65 6467 655f      nx.set_edge_
-00000650: 6174 7472 6962 7574 6573 2867 7261 7068  attributes(graph
-00000660: 2c20 7363 6f72 655f 7661 6c75 6573 2c20  , score_values, 
-00000670: 6e61 6d65 3d27 7363 6f72 6527 290d 0a20  name='score').. 
-00000680: 2020 206e 782e 7365 745f 6564 6765 5f61     nx.set_edge_a
-00000690: 7474 7269 6275 7465 7328 6772 6170 682c  ttributes(graph,
-000006a0: 2062 6163 6b62 6f6e 655f 6564 6765 732c   backbone_edges,
-000006b0: 206e 616d 653d 2768 6967 685f 7361 6c69   name='high_sali
-000006c0: 656e 6365 5f73 6b65 6c65 746f 6e27 290d  ence_skeleton').
-000006d0: 0a0d 0a20 2020 2023 2066 6f72 2075 2c76  ...    # for u,v
-000006e0: 2069 6e20 6772 6170 682e 6564 6765 7328   in graph.edges(
-000006f0: 293a 0d0a 2020 2020 2320 2020 2020 6966  ):..    #     if
-00000700: 2067 7261 7068 5b75 5d5b 765d 5b27 7363   graph[u][v]['sc
-00000710: 6f72 6527 5d3e 3d30 2e38 3a0d 0a20 2020  ore']>=0.8:..   
-00000720: 2023 2020 2020 2020 2020 2067 7261 7068   #         graph
-00000730: 5b75 5d5b 765d 5b27 6869 6768 5f73 616c  [u][v]['high_sal
-00000740: 6965 6e63 655f 736b 656c 6574 6f6e 275d  ience_skeleton']
-00000750: 203d 2054 7275 650d 0a20 2020 2023 2020   = True..    #  
-00000760: 2020 2065 6c73 653a 0d0a 2020 2020 2320     else:..    # 
-00000770: 2020 2020 2020 2020 6772 6170 685b 755d          graph[u]
-00000780: 5b76 5d5b 2768 6967 685f 7361 6c69 656e  [v]['high_salien
-00000790: 6365 5f73 6b65 6c65 746f 6e27 5d20 3d20  ce_skeleton'] = 
-000007a0: 4661 6c73 650d 0a20 2020 2072 6574 7572  False..    retur
-000007b0: 6e20 4261 636b 626f 6e65 2867 7261 7068  n Backbone(graph
-000007c0: 2c20 6e61 6d65 3d22 4869 6768 2053 616c  , name="High Sal
-000007d0: 6965 6e63 6520 536b 656c 6574 6f6e 2046  ience Skeleton F
-000007e0: 696c 7465 7222 2c20 636f 6c75 6d6e 3d22  ilter", column="
-000007f0: 6869 6768 5f73 616c 6965 6e63 655f 736b  high_salience_sk
-00000800: 656c 6574 6f6e 222c 2061 7363 656e 6469  eleton", ascendi
-00000810: 6e67 3d46 616c 7365 2c20 6669 6c74 6572  ng=False, filter
-00000820: 733d 5b62 6f6f 6c65 616e 5f66 696c 7465  s=[boolean_filte
-00000830: 722c 2074 6872 6573 686f 6c64 5f66 696c  r, threshold_fil
-00000840: 7465 722c 2066 7261 6374 696f 6e5f 6669  ter, fraction_fi
-00000850: 6c74 6572 5d29 0d0a                      lter])..
+00000000: 696d 706f 7274 206e 6574 776f 726b 7820  import networkx 
+00000010: 6173 206e 780d 0a69 6d70 6f72 7420 7061  as nx..import pa
+00000020: 6e64 6173 2061 7320 7064 0d0a 6672 6f6d  ndas as pd..from
+00000030: 206e 6574 626f 6e65 2e62 6163 6b62 6f6e   netbone.backbon
+00000040: 6520 696d 706f 7274 2042 6163 6b62 6f6e  e import Backbon
+00000050: 650d 0a66 726f 6d20 6e65 7462 6f6e 652e  e..from netbone.
+00000060: 6669 6c74 6572 7320 696d 706f 7274 2062  filters import b
+00000070: 6f6f 6c65 616e 5f66 696c 7465 722c 2074  oolean_filter, t
+00000080: 6872 6573 686f 6c64 5f66 696c 7465 722c  hreshold_filter,
+00000090: 2066 7261 6374 696f 6e5f 6669 6c74 6572   fraction_filter
+000000a0: 0d0a 0d0a 0d0a 6465 6620 6869 6768 5f73  ......def high_s
+000000b0: 616c 6965 6e63 655f 736b 656c 6574 6f6e  alience_skeleton
+000000c0: 2864 6174 6129 3a0d 0a20 2020 2069 6620  (data):..    if 
+000000d0: 6973 696e 7374 616e 6365 2864 6174 612c  isinstance(data,
+000000e0: 2070 642e 4461 7461 4672 616d 6529 3a0d   pd.DataFrame):.
+000000f0: 0a20 2020 2020 2020 2067 7261 7068 203d  .        graph =
+00000100: 206e 782e 6672 6f6d 5f70 616e 6461 735f   nx.from_pandas_
+00000110: 6564 6765 6c69 7374 2864 6174 612c 2065  edgelist(data, e
+00000120: 6467 655f 6174 7472 3d27 7765 6967 6874  dge_attr='weight
+00000130: 272c 2063 7265 6174 655f 7573 696e 673d  ', create_using=
+00000140: 6e78 2e47 7261 7068 2829 290d 0a20 2020  nx.Graph())..   
+00000150: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00000160: 2864 6174 612c 206e 782e 4772 6170 6829  (data, nx.Graph)
+00000170: 3a0d 0a20 2020 2020 2020 2067 7261 7068  :..        graph
+00000180: 203d 2064 6174 612e 636f 7079 2829 0d0a   = data.copy()..
+00000190: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000001a0: 2020 2070 7269 6e74 2822 6461 7461 2073     print("data s
+000001b0: 686f 756c 6420 6265 2061 2070 616e 6164  hould be a panad
+000001c0: 7320 6461 7461 6672 616d 6520 6f72 206e  s dataframe or n
+000001d0: 7820 6772 6170 6822 290d 0a20 2020 2020  x graph")..     
+000001e0: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
+000001f0: 2077 6573 203d 206e 782e 6765 745f 6564   wes = nx.get_ed
+00000200: 6765 5f61 7474 7269 6275 7465 7328 6772  ge_attributes(gr
+00000210: 6170 682c 2027 7765 6967 6874 2729 0d0a  aph, 'weight')..
+00000220: 2020 2020 7661 6c75 6573 203d 207b 7061      values = {pa
+00000230: 6972 3a20 3120 2f20 7765 735b 7061 6972  ir: 1 / wes[pair
+00000240: 5d20 666f 7220 7061 6972 2069 6e20 7765  ] for pair in we
+00000250: 737d 0d0a 2020 2020 6e78 2e73 6574 5f65  s}..    nx.set_e
+00000260: 6467 655f 6174 7472 6962 7574 6573 2867  dge_attributes(g
+00000270: 7261 7068 2c20 7661 6c75 6573 2c20 6e61  raph, values, na
+00000280: 6d65 3d27 6469 7374 616e 6365 2729 0d0a  me='distance')..
+00000290: 0d0a 2020 2020 6e78 2e73 6574 5f65 6467  ..    nx.set_edg
+000002a0: 655f 6174 7472 6962 7574 6573 2867 7261  e_attributes(gra
+000002b0: 7068 2c20 302c 206e 616d 653d 2773 616c  ph, 0, name='sal
+000002c0: 6965 6e63 6527 290d 0a0d 0a20 2020 2066  ience')....    f
+000002d0: 6f72 2073 6f75 7263 6520 696e 2067 7261  or source in gra
+000002e0: 7068 2e6e 6f64 6573 2829 3a0d 0a20 2020  ph.nodes():..   
+000002f0: 2020 2020 2074 7265 6520 3d20 6e78 2e73       tree = nx.s
+00000300: 696e 676c 655f 736f 7572 6365 5f64 696a  ingle_source_dij
+00000310: 6b73 7472 6128 6772 6170 682c 2073 6f75  kstra(graph, sou
+00000320: 7263 652c 2063 7574 6f66 663d 4e6f 6e65  rce, cutoff=None
+00000330: 2c20 7765 6967 6874 3d27 6469 7374 616e  , weight='distan
+00000340: 6365 2729 5b31 5d0d 0a20 2020 2020 2020  ce')[1]..       
+00000350: 206e 6f64 655f 7472 6565 5f73 636f 7265   node_tree_score
+00000360: 7320 3d20 6469 6374 2829 0d0a 0d0a 2020  s = dict()....  
+00000370: 2020 2020 2020 7061 7468 7320 3d20 6c69        paths = li
+00000380: 7374 2874 7265 652e 7661 6c75 6573 2829  st(tree.values()
+00000390: 295b 313a 5d0d 0a20 2020 2020 2020 2066  )[1:]..        f
+000003a0: 6f72 2070 6174 6820 696e 2070 6174 6873  or path in paths
+000003b0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+000003c0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+000003d0: 6e28 7061 7468 2920 2d20 3129 3a0d 0a20  n(path) - 1):.. 
+000003e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000003f0: 6f64 655f 7472 6565 5f73 636f 7265 735b  ode_tree_scores[
+00000400: 2870 6174 685b 695d 2c20 7061 7468 5b69  (path[i], path[i
+00000410: 202b 2031 5d29 5d20 3d20 310d 0a0d 0a20   + 1])] = 1.... 
+00000420: 2020 2020 2020 2066 6f72 2075 2c20 7620         for u, v 
+00000430: 696e 206e 6f64 655f 7472 6565 5f73 636f  in node_tree_sco
+00000440: 7265 733a 0d0a 2020 2020 2020 2020 2020  res:..          
+00000450: 2020 6772 6170 685b 755d 5b76 5d5b 2773    graph[u][v]['s
+00000460: 616c 6965 6e63 6527 5d20 2b3d 2031 0d0a  alience'] += 1..
+00000470: 0d0a 2020 2020 7363 6f72 6573 203d 206e  ..    scores = n
+00000480: 782e 6765 745f 6564 6765 5f61 7474 7269  x.get_edge_attri
+00000490: 6275 7465 7328 6772 6170 682c 2027 7361  butes(graph, 'sa
+000004a0: 6c69 656e 6365 2729 0d0a 2020 2020 4e20  lience')..    N 
+000004b0: 3d20 6c65 6e28 6772 6170 6829 0d0a 2020  = len(graph)..  
+000004c0: 2020 7363 6f72 655f 7661 6c75 6573 203d    score_values =
+000004d0: 2064 6963 7428 290d 0a20 2020 2062 6163   dict()..    bac
+000004e0: 6b62 6f6e 655f 6564 6765 7320 3d20 6469  kbone_edges = di
+000004f0: 6374 2829 0d0a 2020 2020 666f 7220 7061  ct()..    for pa
+00000500: 6972 2069 6e20 7363 6f72 6573 3a0d 0a20  ir in scores:.. 
+00000510: 2020 2020 2020 2073 636f 7265 5f76 616c         score_val
+00000520: 7565 735b 7061 6972 5d20 3d20 7363 6f72  ues[pair] = scor
+00000530: 6573 5b70 6169 725d 202f 204e 0d0a 2020  es[pair] / N..  
+00000540: 2020 2020 2020 6966 2073 636f 7265 735b        if scores[
+00000550: 7061 6972 5d20 2f20 4e20 3e20 302e 383a  pair] / N > 0.8:
+00000560: 0d0a 2020 2020 2020 2020 2020 2020 6261  ..            ba
+00000570: 636b 626f 6e65 5f65 6467 6573 5b70 6169  ckbone_edges[pai
+00000580: 725d 203d 2054 7275 650d 0a20 2020 2020  r] = True..     
+00000590: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+000005a0: 2020 2020 2020 6261 636b 626f 6e65 5f65        backbone_e
+000005b0: 6467 6573 5b70 6169 725d 203d 2046 616c  dges[pair] = Fal
+000005c0: 7365 0d0a 0d0a 2020 2020 2020 2020 2020  se....          
+000005d0: 2020 2320 7363 6f72 655f 7661 6c75 6573    # score_values
+000005e0: 203d 207b 7061 6972 3a73 636f 7265 735b   = {pair:scores[
+000005f0: 7061 6972 5d2f 4e20 666f 7220 7061 6972  pair]/N for pair
+00000600: 2069 6e20 7363 6f72 6573 7d0d 0a20 2020   in scores}..   
+00000610: 206e 782e 7365 745f 6564 6765 5f61 7474   nx.set_edge_att
+00000620: 7269 6275 7465 7328 6772 6170 682c 2073  ributes(graph, s
+00000630: 636f 7265 5f76 616c 7565 732c 206e 616d  core_values, nam
+00000640: 653d 2773 616c 6965 6e63 6527 290d 0a20  e='salience').. 
+00000650: 2020 206e 782e 7365 745f 6564 6765 5f61     nx.set_edge_a
+00000660: 7474 7269 6275 7465 7328 6772 6170 682c  ttributes(graph,
+00000670: 2062 6163 6b62 6f6e 655f 6564 6765 732c   backbone_edges,
+00000680: 206e 616d 653d 2769 6e5f 6261 636b 626f   name='in_backbo
+00000690: 6e65 2729 0d0a 0d0a 2020 2020 7265 7475  ne')....    retu
+000006a0: 726e 2042 6163 6b62 6f6e 6528 6772 6170  rn Backbone(grap
+000006b0: 682c 206d 6574 686f 645f 6e61 6d65 3d22  h, method_name="
+000006c0: 4869 6768 2053 616c 6965 6e63 6520 536b  High Salience Sk
+000006d0: 656c 6574 6f6e 2046 696c 7465 7222 2c20  eleton Filter", 
+000006e0: 7072 6f70 6572 7479 5f6e 616d 653d 2273  property_name="s
+000006f0: 616c 6965 6e63 6522 2c0d 0a20 2020 2020  alience",..     
+00000700: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00000710: 7363 656e 6469 6e67 3d46 616c 7365 2c20  scending=False, 
+00000720: 636f 6d70 6174 6962 6c65 5f66 696c 7465  compatible_filte
+00000730: 7273 3d5b 626f 6f6c 6561 6e5f 6669 6c74  rs=[boolean_filt
+00000740: 6572 2c20 7468 7265 7368 6f6c 645f 6669  er, threshold_fi
+00000750: 6c74 6572 2c20 6672 6163 7469 6f6e 5f66  lter, fraction_f
+00000760: 696c 7465 725d 2c0d 0a20 2020 2020 2020  ilter],..       
+00000770: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00000780: 7465 725f 6f6e 3d27 4564 6765 7327 290d  ter_on='Edges').
+00000790: 0a                                       .
```

### Comparing `netbone-0.2.1.1/netbone/structural/maximum_spanning_tree.py` & `netbone-0.2.2/netbone/structural/maximum_spanning_tree.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import networkx as nx
 import pandas as pd
 from netbone.backbone import Backbone
 from netbone.filters import boolean_filter
+from netbone.utils.utils import edge_properties
 # algo: minimum_spanning_tree
 # calculating MSP
 
 def maximum_spanning_tree(data):
     if isinstance(data, pd.DataFrame):
-        G = nx.from_pandas_edgelist(data, edge_attr='weight', create_using=nx.Graph())
+        g = nx.from_pandas_edgelist(data, edge_attr=edge_properties(data))
     elif isinstance(data, nx.Graph):
-        G = data.copy()
+        g = data.copy()
     else:
         print("data should be a panads dataframe or nx graph")
         return
 
+    nx.set_edge_attributes(g, True, name='in_backbone')
+    msp = nx.maximum_spanning_tree(g, weight='weight')
 
-    df = nx.to_pandas_edgelist((G))
-    df['distance'] = df.apply(lambda row : 1/row['weight'], axis = 1)
+    missing_edges = {edge: {"in_backbone": False} for edge in set(g.edges()).difference(set(msp.edges()))}
+    nx.set_edge_attributes(g, missing_edges)
 
-    nx.set_edge_attributes(G, nx.get_edge_attributes(nx.from_pandas_edgelist(df, edge_attr='distance'), 'distance'), name='distance')
-    msp = nx.minimum_spanning_tree(G, weight='distance')
-    nx.set_edge_attributes(G, True, name='msp_backbone')
-
-    missing_edges = {edge: {"msp_backbone": False} for edge in set(G.edges()).difference(set(msp.edges()))}
-    nx.set_edge_attributes(G, missing_edges)
-
-    return Backbone(G, name="Maximum Spanning Tree", column="msp_backbone", ascending=False, filters=[boolean_filter])
+    return Backbone(g, method_name="Maximum Spanning Tree", property_name="weight", ascending=False, compatible_filters=[boolean_filter], filter_on='Edges')
```

### Comparing `netbone-0.2.1.1/netbone/utils/utils.py` & `netbone-0.2.2/netbone/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     if increasing:
         x = -np.sort(-np.array(values))
     else:
         x = np.sort(values)
     y = np.arange(1, len(x) + 1)/len(x)
 
     df = pd.DataFrame(index=x)
-    df.index.name = name
+    df.index.method_name = name
     df[method] = y
     return df
 
 def edge_properties(df):
     columns = list(df.columns)
     columns.remove('source')
     columns.remove('target')
```

### Comparing `netbone-0.2.1.1/netbone/visualize.py` & `netbone-0.2.2/netbone/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 
         axs.spines['bottom'].set_color('0.3')
         axs.spines['top'].set_color('0.3')
         axs.spines['right'].set_color('0.3')
         axs.spines['left'].set_color('0.3')
 
 
-        axs.set_xlabel(df[method].index.name)
+        axs.set_xlabel(prop)
         axs.set_ylabel('P')
 
         axs.legend(loc='center left', bbox_to_anchor=(1.04,0.5))
         fig.suptitle(title)
 
         # plt.tight_layout()
         plt.show()
```

### Comparing `netbone-0.2.1.1/netbone.egg-info/PKG-INFO` & `netbone-0.2.2/netbone.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbone
-Version: 0.2.1.1
+Version: 0.2.2
 Summary: A python package for extracting network backbones from simple weighted networks
 Home-page: https://gitlab.liris.cnrs.fr/coregraphie/netbone
 Author: Ali Yassin
 Author-email: aliyassin4@hotmail.com
 License: MIT
 Keywords: backbone network
 Description-Content-Type: text/markdown
@@ -14,15 +14,16 @@
 
 NetBone is a Python library for extracting network backbones from simple weighted networks.
 
 ## Features
 
 - Extract network backbones from simple weighted networks
 - Contains six statistical methods for extracting backbones
-- Contains seven structural methods for extracting backbones
+- Contains thirteen structural methods for extracting backbones
+- Contains one hybrid method for extracting backbones
 - Includes three filters for extracting the backbone: boolean filter, threshold filter, and fraction filter
 - Built-in methods for comparing backbones with each other
 - Option to use custom comparison methods
 - Visualization tools to display the results of the comparison
```

### Comparing `netbone-0.2.1.1/setup.py` & `netbone-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netbone',
     packages=find_packages(),
-    version='0.2.1.1',
+    version='0.2.2',
     author='Ali Yassin',
     license='MIT',
     author_email='aliyassin4@hotmail.com',
     url='https://gitlab.liris.cnrs.fr/coregraphie/netbone',
     keywords='backbone network',
     description='A python package for extracting network backbones from simple weighted networks',
     long_description=long_description,
```

