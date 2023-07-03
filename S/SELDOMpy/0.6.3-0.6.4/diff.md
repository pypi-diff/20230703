# Comparing `tmp/SELDOMpy-0.6.3.tar.gz` & `tmp/SELDOMpy-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.6.3.tar", last modified: Thu Jun 29 16:31:10 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.6.4.tar", last modified: Mon Jul  3 15:44:32 2023, max compression
```

## Comparing `SELDOMpy-0.6.3.tar` & `SELDOMpy-0.6.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 16:31:10.785353 SELDOMpy-0.6.3/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.6.3/LICENSE.txt
--rw-rw-rw-   0        0        0      141 2023-06-29 16:31:10.785353 SELDOMpy-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 16:31:10.778355 SELDOMpy-0.6.3/SELDOMpy/
--rw-rw-rw-   0        0        0      388 2023-06-29 07:41:16.000000 SELDOMpy-0.6.3/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:31:10.783353 SELDOMpy-0.6.3/SELDOMpy/build/
--rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.6.3/SELDOMpy/build/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.6.3/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.6.3/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.6.3/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.6.3/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.6.3/SELDOMpy/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.6.3/SELDOMpy/opt_mealpy.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.6.3/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.6.3/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.6.3/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.6.3/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-29 16:31:10.783353 SELDOMpy-0.6.3/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      141 2023-06-29 16:31:10.000000 SELDOMpy-0.6.3/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-06-29 16:31:10.000000 SELDOMpy-0.6.3/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 16:31:10.000000 SELDOMpy-0.6.3/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-29 16:31:10.000000 SELDOMpy-0.6.3/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-29 16:31:10.000000 SELDOMpy-0.6.3/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-29 16:31:10.785353 SELDOMpy-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     3084 2023-06-29 16:30:52.000000 SELDOMpy-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:44:32.950781 SELDOMpy-0.6.4/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.6.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      641 2023-07-03 15:44:32.950781 SELDOMpy-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 15:44:32.918749 SELDOMpy-0.6.4/SELDOMpy/
+-rw-rw-rw-   0        0        0      390 2023-07-03 07:13:49.000000 SELDOMpy-0.6.4/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:44:32.948781 SELDOMpy-0.6.4/SELDOMpy/build/
+-rw-rw-rw-   0        0        0        0 2023-06-28 11:40:30.000000 SELDOMpy-0.6.4/SELDOMpy/build/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.6.4/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1271 2023-04-14 17:44:15.000000 SELDOMpy-0.6.4/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.6.4/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.6.4/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.6.4/SELDOMpy/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.6.4/SELDOMpy/optimization.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.6.4/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.6.4/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.6.4/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.6.4/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:44:32.947745 SELDOMpy-0.6.4/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      641 2023-07-03 15:44:32.000000 SELDOMpy-0.6.4/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-07-03 15:44:32.000000 SELDOMpy-0.6.4/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 15:44:32.000000 SELDOMpy-0.6.4/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-03 15:44:32.000000 SELDOMpy-0.6.4/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-03 15:44:32.000000 SELDOMpy-0.6.4/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-03 15:44:32.951778 SELDOMpy-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     2621 2023-07-03 15:43:19.000000 SELDOMpy-0.6.4/setup.py
```

### Comparing `SELDOMpy-0.6.3/LICENSE.txt` & `SELDOMpy-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/buildmim.py` & `SELDOMpy-0.6.4/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/extras.py` & `SELDOMpy-0.6.4/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/gen_exps.py` & `SELDOMpy-0.6.4/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.6.4/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.6.4/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/opt_mealpy.py` & `SELDOMpy-0.6.4/SELDOMpy/optimization.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/plot_results.py` & `SELDOMpy-0.6.4/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.6.4/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.6.4/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.6.4/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.6.3/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.6.4/SELDOMpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup.py
 SELDOMpy/__init__.py
 SELDOMpy/buildmim.py
 SELDOMpy/extras.py
 SELDOMpy/gen_exps.py
 SELDOMpy/getLBODEmodel.py
 SELDOMpy/getRandomLBODEmodel.py
-SELDOMpy/opt_mealpy.py
+SELDOMpy/optimization.py
 SELDOMpy/plot_results.py
 SELDOMpy/reduce_fun.py
 SELDOMpy/simulate_logic_based_ode.py
 SELDOMpy/simulate_logic_based_ode_obs.py
 SELDOMpy.egg-info/PKG-INFO
 SELDOMpy.egg-info/SOURCES.txt
 SELDOMpy.egg-info/dependency_links.txt
```

