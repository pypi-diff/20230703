# Comparing `tmp/dapla_toolbelt-1.7.1.tar.gz` & `tmp/dapla_toolbelt-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt-1.7.1.tar", max compression
+gzip compressed data, was "dapla_toolbelt-1.8.0.tar", max compression
```

## Comparing `dapla_toolbelt-1.7.1.tar` & `dapla_toolbelt-1.8.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1074 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/LICENSE
--rw-r--r--   0        0        0     6602 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/README.md
--rw-r--r--   0        0        0      401 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/__init__.py
--rw-r--r--   0        0        0     2906 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/auth.py
--rw-r--r--   0        0        0     1576 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/backports.py
--rw-r--r--   0        0        0     1537 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/collector.py
--rw-r--r--   0        0        0     4120 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/converter.py
--rw-r--r--   0        0        0     4185 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/doctor.py
--rw-r--r--   0        0        0     5550 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/files.py
--rw-r--r--   0        0        0     1861 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/gcs.py
--rw-r--r--   0        0        0     2887 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/guardian.py
--rw-r--r--   0        0        0     1140 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/jupyterhub.py
--rw-r--r--   0        0        0     4322 2023-06-13 09:23:10.437530 dapla_toolbelt-1.7.1/dapla/pandas.py
--rw-r--r--   0        0        0     6031 2023-06-13 09:23:10.441530 dapla_toolbelt-1.7.1/dapla/pubsub.py
--rw-r--r--   0        0        0        0 2023-06-13 09:23:10.441530 dapla_toolbelt-1.7.1/dapla/spark/__init__.py
--rw-r--r--   0        0        0      378 2023-06-13 09:23:10.441530 dapla_toolbelt-1.7.1/dapla/spark/sparkui.py
--rw-r--r--   0        0        0     3139 2023-06-13 09:23:10.441530 dapla_toolbelt-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     7730 1970-01-01 00:00:00.000000 dapla_toolbelt-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/LICENSE
+-rw-r--r--   0        0        0     6602 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/__init__.py
+-rw-r--r--   0        0        0     2906 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/auth.py
+-rw-r--r--   0        0        0     1576 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/backports.py
+-rw-r--r--   0        0        0     1537 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/collector.py
+-rw-r--r--   0        0        0     4120 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/converter.py
+-rw-r--r--   0        0        0     4185 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/doctor.py
+-rw-r--r--   0        0        0     5550 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/files.py
+-rw-r--r--   0        0        0     1861 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/gcs.py
+-rw-r--r--   0        0        0     1060 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/git.py
+-rw-r--r--   0        0        0     2887 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/guardian.py
+-rw-r--r--   0        0        0     1140 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/jupyterhub.py
+-rw-r--r--   0        0        0     4322 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/pandas.py
+-rw-r--r--   0        0        0     6031 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/pubsub.py
+-rw-r--r--   0        0        0        0 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/spark/__init__.py
+-rw-r--r--   0        0        0      378 2023-07-03 08:37:46.560566 dapla_toolbelt-1.8.0/dapla/spark/sparkui.py
+-rw-r--r--   0        0        0     3139 2023-07-03 08:37:46.564566 dapla_toolbelt-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7730 1970-01-01 00:00:00.000000 dapla_toolbelt-1.8.0/PKG-INFO
```

### Comparing `dapla_toolbelt-1.7.1/LICENSE` & `dapla_toolbelt-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/README.md` & `dapla_toolbelt-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/auth.py` & `dapla_toolbelt-1.8.0/dapla/auth.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/backports.py` & `dapla_toolbelt-1.8.0/dapla/backports.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/collector.py` & `dapla_toolbelt-1.8.0/dapla/collector.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/converter.py` & `dapla_toolbelt-1.8.0/dapla/converter.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/doctor.py` & `dapla_toolbelt-1.8.0/dapla/doctor.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/files.py` & `dapla_toolbelt-1.8.0/dapla/files.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/gcs.py` & `dapla_toolbelt-1.8.0/dapla/gcs.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/guardian.py` & `dapla_toolbelt-1.8.0/dapla/guardian.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/jupyterhub.py` & `dapla_toolbelt-1.8.0/dapla/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/pandas.py` & `dapla_toolbelt-1.8.0/dapla/pandas.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/dapla/pubsub.py` & `dapla_toolbelt-1.8.0/dapla/pubsub.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.7.1/pyproject.toml` & `dapla_toolbelt-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt"
-version = "1.7.1"
+version = "1.8.0"
 description = "Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called Dapla"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt"
 
 classifiers = [
```

### Comparing `dapla_toolbelt-1.7.1/PKG-INFO` & `dapla_toolbelt-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt
-Version: 1.7.1
+Version: 1.8.0
 Summary: Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

