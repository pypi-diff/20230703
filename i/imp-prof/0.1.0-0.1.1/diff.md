# Comparing `tmp/imp-prof-0.1.0.tar.gz` & `tmp/imp-prof-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imp-prof-0.1.0.tar", last modified: Mon Jul  3 12:35:15 2023, max compression
+gzip compressed data, was "imp-prof-0.1.1.tar", last modified: Mon Jul  3 14:04:52 2023, max compression
```

## Comparing `imp-prof-0.1.0.tar` & `imp-prof-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-07-03 12:35:15.272929 imp-prof-0.1.0/
--rw-r--r--   0 trval     (1000) trval     (1000)      656 2022-11-08 14:01:21.000000 imp-prof-0.1.0/CHANGELOG.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1517 2022-11-08 14:01:21.000000 imp-prof-0.1.0/LICENSE
--rw-r--r--   0 trval     (1000) trval     (1000)       56 2022-11-08 14:01:21.000000 imp-prof-0.1.0/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     1810 2023-07-03 12:35:15.269596 imp-prof-0.1.0/PKG-INFO
--rw-r--r--   0 trval     (1000) trval     (1000)      902 2022-11-08 14:01:21.000000 imp-prof-0.1.0/README.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1616 2023-07-03 11:36:52.000000 imp-prof-0.1.0/pyproject.toml
--rw-r--r--   0 trval     (1000) trval     (1000)      173 2022-11-08 14:01:21.000000 imp-prof-0.1.0/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-07-03 12:35:15.272929 imp-prof-0.1.0/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-07-03 12:35:15.269596 imp-prof-0.1.0/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-07-03 12:35:15.269596 imp-prof-0.1.0/src/imp_prof/
--rw-r--r--   0 trval     (1000) trval     (1000)      227 2022-11-08 14:01:21.000000 imp-prof-0.1.0/src/imp_prof/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)      989 2023-05-30 09:27:08.000000 imp-prof-0.1.0/src/imp_prof/default_config.py
--rw-r--r--   0 trval     (1000) trval     (1000)     4414 2023-05-30 09:27:08.000000 imp-prof-0.1.0/src/imp_prof/envs.py
--rw-r--r--   0 trval     (1000) trval     (1000)      531 2022-11-08 14:01:21.000000 imp-prof-0.1.0/src/imp_prof/info.py
--rw-r--r--   0 trval     (1000) trval     (1000)     4092 2023-05-30 09:27:08.000000 imp-prof-0.1.0/src/imp_prof/loader.py
--rw-r--r--   0 trval     (1000) trval     (1000)     3956 2023-05-30 09:27:08.000000 imp-prof-0.1.0/src/imp_prof/log.py
--rw-r--r--   0 trval     (1000) trval     (1000)     2363 2023-05-31 11:58:08.000000 imp-prof-0.1.0/src/imp_prof/main.py
--rw-r--r--   0 trval     (1000) trval     (1000)    10172 2023-05-31 11:58:08.000000 imp-prof-0.1.0/src/imp_prof/metric.py
--rw-r--r--   0 trval     (1000) trval     (1000)     2410 2023-05-30 12:53:02.000000 imp-prof-0.1.0/src/imp_prof/routes.py
--rw-r--r--   0 trval     (1000) trval     (1000)      580 2023-05-30 09:27:08.000000 imp-prof-0.1.0/src/imp_prof/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-07-03 12:35:15.269596 imp-prof-0.1.0/src/imp_prof.egg-info/
--rw-r--r--   0 trval     (1000) trval     (1000)     1810 2023-07-03 12:35:15.000000 imp-prof-0.1.0/src/imp_prof.egg-info/PKG-INFO
--rw-r--r--   0 trval     (1000) trval     (1000)      483 2023-07-03 12:35:15.000000 imp-prof-0.1.0/src/imp_prof.egg-info/SOURCES.txt
--rw-r--r--   0 trval     (1000) trval     (1000)        1 2023-07-03 12:35:15.000000 imp-prof-0.1.0/src/imp_prof.egg-info/dependency_links.txt
--rw-r--r--   0 trval     (1000) trval     (1000)      180 2023-07-03 12:35:15.000000 imp-prof-0.1.0/src/imp_prof.egg-info/requires.txt
--rw-r--r--   0 trval     (1000) trval     (1000)        9 2023-07-03 12:35:15.000000 imp-prof-0.1.0/src/imp_prof.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-07-03 14:04:52.930243 imp-prof-0.1.1/
+-rw-r--r--   0 trval     (1000) trval     (1000)      668 2023-07-03 14:04:36.000000 imp-prof-0.1.1/CHANGELOG.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1517 2022-11-08 14:01:21.000000 imp-prof-0.1.1/LICENSE
+-rw-r--r--   0 trval     (1000) trval     (1000)       56 2022-11-08 14:01:21.000000 imp-prof-0.1.1/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     1810 2023-07-03 14:04:52.930243 imp-prof-0.1.1/PKG-INFO
+-rw-r--r--   0 trval     (1000) trval     (1000)      902 2022-11-08 14:01:21.000000 imp-prof-0.1.1/README.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1616 2023-07-03 11:36:52.000000 imp-prof-0.1.1/pyproject.toml
+-rw-r--r--   0 trval     (1000) trval     (1000)      173 2022-11-08 14:01:21.000000 imp-prof-0.1.1/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-07-03 14:04:52.930243 imp-prof-0.1.1/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-07-03 14:04:52.926910 imp-prof-0.1.1/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-07-03 14:04:52.930243 imp-prof-0.1.1/src/imp_prof/
+-rw-r--r--   0 trval     (1000) trval     (1000)      239 2023-07-03 14:00:51.000000 imp-prof-0.1.1/src/imp_prof/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)      989 2023-05-30 09:27:08.000000 imp-prof-0.1.1/src/imp_prof/default_config.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     4414 2023-05-30 09:27:08.000000 imp-prof-0.1.1/src/imp_prof/envs.py
+-rw-r--r--   0 trval     (1000) trval     (1000)      531 2023-07-03 14:04:13.000000 imp-prof-0.1.1/src/imp_prof/info.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     4092 2023-05-30 09:27:08.000000 imp-prof-0.1.1/src/imp_prof/loader.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     3956 2023-05-30 09:27:08.000000 imp-prof-0.1.1/src/imp_prof/log.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     2363 2023-05-31 11:58:08.000000 imp-prof-0.1.1/src/imp_prof/main.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    10172 2023-05-31 11:58:08.000000 imp-prof-0.1.1/src/imp_prof/metric.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     2410 2023-05-30 12:53:02.000000 imp-prof-0.1.1/src/imp_prof/routes.py
+-rw-r--r--   0 trval     (1000) trval     (1000)      580 2023-05-30 09:27:08.000000 imp-prof-0.1.1/src/imp_prof/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-07-03 14:04:52.930243 imp-prof-0.1.1/src/imp_prof.egg-info/
+-rw-r--r--   0 trval     (1000) trval     (1000)     1810 2023-07-03 14:04:52.000000 imp-prof-0.1.1/src/imp_prof.egg-info/PKG-INFO
+-rw-r--r--   0 trval     (1000) trval     (1000)      483 2023-07-03 14:04:52.000000 imp-prof-0.1.1/src/imp_prof.egg-info/SOURCES.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)        1 2023-07-03 14:04:52.000000 imp-prof-0.1.1/src/imp_prof.egg-info/dependency_links.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)      180 2023-07-03 14:04:52.000000 imp-prof-0.1.1/src/imp_prof.egg-info/requires.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)        9 2023-07-03 14:04:52.000000 imp-prof-0.1.1/src/imp_prof.egg-info/top_level.txt
```

### Comparing `imp-prof-0.1.0/CHANGELOG.md` & `imp-prof-0.1.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.1]
+
 ### Added
 
 - Pack project for PyPI.
 - Refactor `messaging` into package with prepared `BlockingPublisher` with use of `pika`.
 - Separate out common types definition into `imp_prof.types` module.
 
 ## [0.1.0]
```

### Comparing `imp-prof-0.1.0/LICENSE` & `imp-prof-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/PKG-INFO` & `imp-prof-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imp-prof
-Version: 0.1.0
+Version: 0.1.1
 Summary: Imp-prof serves to collect and publish prometheus metrics from pre-forked server workers.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://gitlab.kajot.cz/online-casino/backend/imp-prof
 Project-URL: Bug Tracker, https://gitlab.kajot.cz/online-casino/backend/imp-prof
 Keywords: prometheus,fastapi,api,rest,profiling,rabbitmq,python,pika,metrics
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `imp-prof-0.1.0/README.md` & `imp-prof-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/pyproject.toml` & `imp-prof-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/src/imp_prof/default_config.py` & `imp-prof-0.1.1/src/imp_prof/default_config.py`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/src/imp_prof/envs.py` & `imp-prof-0.1.1/src/imp_prof/envs.py`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/src/imp_prof/info.py` & `imp-prof-0.1.1/src/imp_prof/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name = "Imp-Prof"
 name_unify = name.lower()
-version = (0, 1, 0)
+version = (0, 1, 1)
 __version__ = ".".join(map(str, version))
-__build__ = "2022-10-14T13:30:00.000+00:00"
+__build__ = "2023-07-03T15:00:00.000+00:00"
 __author__ = "[tom trval](https://github.com/Ryu-CZ)"
 description = (
     "Imp consumes log messages from [RabbitMQ](https://www.rabbitmq.com/) into [Prometheus](https://prometheus.io/) "
     "metrics published on API to be scraped "
 )
 contact = {
     "name": "support",
```

### Comparing `imp-prof-0.1.0/src/imp_prof/loader.py` & `imp-prof-0.1.1/src/imp_prof/loader.py`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/src/imp_prof/log.py` & `imp-prof-0.1.1/src/imp_prof/log.py`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/src/imp_prof/main.py` & `imp-prof-0.1.1/src/imp_prof/main.py`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/src/imp_prof/metric.py` & `imp-prof-0.1.1/src/imp_prof/metric.py`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/src/imp_prof/routes.py` & `imp-prof-0.1.1/src/imp_prof/routes.py`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/src/imp_prof/types.py` & `imp-prof-0.1.1/src/imp_prof/types.py`

 * *Files identical despite different names*

### Comparing `imp-prof-0.1.0/src/imp_prof.egg-info/PKG-INFO` & `imp-prof-0.1.1/src/imp_prof.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imp-prof
-Version: 0.1.0
+Version: 0.1.1
 Summary: Imp-prof serves to collect and publish prometheus metrics from pre-forked server workers.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://gitlab.kajot.cz/online-casino/backend/imp-prof
 Project-URL: Bug Tracker, https://gitlab.kajot.cz/online-casino/backend/imp-prof
 Keywords: prometheus,fastapi,api,rest,profiling,rabbitmq,python,pika,metrics
 Classifier: License :: OSI Approved :: BSD License
```

