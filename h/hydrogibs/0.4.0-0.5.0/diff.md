# Comparing `tmp/hydrogibs-0.4.0.tar.gz` & `tmp/hydrogibs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.4.0.tar", last modified: Thu Jun 22 14:28:22 2023, max compression
+gzip compressed data, was "hydrogibs-0.5.0.tar", last modified: Mon Jul  3 15:03:19 2023, max compression
```

## Comparing `hydrogibs-0.4.0.tar` & `hydrogibs-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,13 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-22 14:28:22.013080 hydrogibs-0.4.0/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.4.0/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)     1620 2023-06-22 14:28:22.013080 hydrogibs-0.4.0/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.4.0/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-22 14:28:22.013080 hydrogibs-0.4.0/hydrogibs/
--rwxrwxr-x   0 axel      (1000) axel      (1000)    13265 2023-06-22 14:25:57.000000 hydrogibs-0.4.0/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     5258 2023-06-14 13:07:40.000000 hydrogibs-0.4.0/hydrogibs/ModelApp.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1943 2023-06-21 12:15:20.000000 hydrogibs-0.4.0/hydrogibs/ModelTemplate.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     7480 2023-06-04 07:59:58.000000 hydrogibs-0.4.0/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.4.0/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     2228 2023-06-12 15:14:30.000000 hydrogibs-0.4.0/hydrogibs/Riemann.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-05-24 13:52:28.000000 hydrogibs-0.4.0/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      121 2023-06-03 17:06:41.000000 hydrogibs-0.4.0/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     2449 2023-06-09 18:30:47.000000 hydrogibs-0.4.0/hydrogibs/conduites.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1891 2023-06-04 08:00:38.000000 hydrogibs-0.4.0/hydrogibs/constants.py
--rw-rw-r--   0 axel      (1000) axel      (1000)    10932 2023-06-22 14:19:06.000000 hydrogibs-0.4.0/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-22 14:28:22.013080 hydrogibs-0.4.0/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1620 2023-06-22 14:28:21.000000 hydrogibs-0.4.0/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      402 2023-06-22 14:28:22.000000 hydrogibs-0.4.0/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-06-22 14:28:21.000000 hydrogibs-0.4.0/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-06-22 14:28:21.000000 hydrogibs-0.4.0/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      597 2023-06-22 14:28:08.000000 hydrogibs-0.4.0/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-06-22 14:28:22.013080 hydrogibs-0.4.0/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-03 15:03:19.804970 hydrogibs-0.5.0/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.5.0/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      286 2023-07-03 15:03:19.804970 hydrogibs-0.5.0/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.5.0/README.md
+-rw-rw-r--   0 axel      (1000) axel      (1000)      597 2023-06-22 14:28:08.000000 hydrogibs-0.5.0/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-07-03 15:03:19.804970 hydrogibs-0.5.0/setup.cfg
+-rw-rw-r--   0 axel      (1000) axel      (1000)      334 2023-07-03 15:01:49.000000 hydrogibs-0.5.0/setup.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-03 15:03:19.804970 hydrogibs-0.5.0/src/
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-07-03 15:03:19.804970 hydrogibs-0.5.0/src/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      286 2023-07-03 15:03:19.000000 hydrogibs-0.5.0/src/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      189 2023-07-03 15:03:19.000000 hydrogibs-0.5.0/src/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-07-03 15:03:19.000000 hydrogibs-0.5.0/src/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       18 2023-07-03 15:03:19.000000 hydrogibs-0.5.0/src/hydrogibs.egg-info/top_level.txt
```

### Comparing `hydrogibs-0.4.0/LICENSE` & `hydrogibs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.4.0/README.md` & `hydrogibs-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.4.0/pyproject.toml` & `hydrogibs-0.5.0/pyproject.toml`

 * *Files identical despite different names*

