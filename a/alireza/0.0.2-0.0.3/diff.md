# Comparing `tmp/alireza-0.0.2.tar.gz` & `tmp/alireza-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alireza-0.0.2.tar", last modified: Thu Jun 15 16:20:59 2023, max compression
+gzip compressed data, was "alireza-0.0.3.tar", last modified: Mon Jul  3 08:26:02 2023, max compression
```

## Comparing `alireza-0.0.2.tar` & `alireza-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-06-15 16:20:59.942122 alireza-0.0.2/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-06-15 16:20:59.942122 alireza-0.0.2/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-06-14 12:34:33.000000 alireza-0.0.2/README.md
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-06-15 16:20:59.938122 alireza-0.0.2/alireza/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       54 2023-06-15 16:11:41.000000 alireza-0.0.2/alireza/__init__.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     2076 2023-06-14 14:14:09.000000 alireza-0.0.2/alireza/django_tools.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-06-15 16:20:59.938122 alireza-0.0.2/alireza.egg-info/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-06-15 16:20:59.000000 alireza-0.0.2/alireza.egg-info/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      186 2023-06-15 16:20:59.000000 alireza-0.0.2/alireza.egg-info/SOURCES.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-06-15 16:20:59.000000 alireza-0.0.2/alireza.egg-info/dependency_links.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        8 2023-06-15 16:20:59.000000 alireza-0.0.2/alireza.egg-info/top_level.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-06-15 16:20:59.942122 alireza-0.0.2/setup.cfg
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      934 2023-06-15 16:20:12.000000 alireza-0.0.2/setup.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-03 08:26:02.423488 alireza-0.0.3/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-07-03 08:26:02.423488 alireza-0.0.3/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-06-14 12:34:33.000000 alireza-0.0.3/README.md
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-03 08:26:02.423488 alireza-0.0.3/alireza/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       36 2023-07-03 08:11:46.000000 alireza-0.0.3/alireza/__init__.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-03 08:26:02.423488 alireza-0.0.3/alireza/__managers/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       30 2023-07-03 08:06:03.000000 alireza-0.0.3/alireza/__managers/__init__.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1151 2023-07-03 08:02:39.000000 alireza-0.0.3/alireza/__managers/_django_manager.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1719 2023-07-03 08:12:43.000000 alireza-0.0.3/alireza/_django_tools.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-03 08:26:02.423488 alireza-0.0.3/alireza.egg-info/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-07-03 08:26:02.000000 alireza-0.0.3/alireza.egg-info/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      256 2023-07-03 08:26:02.000000 alireza-0.0.3/alireza.egg-info/SOURCES.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-07-03 08:26:02.000000 alireza-0.0.3/alireza.egg-info/dependency_links.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        8 2023-07-03 08:26:02.000000 alireza-0.0.3/alireza.egg-info/top_level.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-07-03 08:26:02.423488 alireza-0.0.3/setup.cfg
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      934 2023-07-03 08:23:33.000000 alireza-0.0.3/setup.py
```

### Comparing `alireza-0.0.2/PKG-INFO` & `alireza-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alireza
-Version: 0.0.2
+Version: 0.0.3
 Summary: Useful tools for python frameworks
 Home-page: UNKNOWN
 Author: Alireza Soroush
 Author-email: alirezasoroush@hotmail.com
 License: UNKNOWN
 Keywords: python,tools,framework,django
 Platform: UNKNOWN
```

### Comparing `alireza-0.0.2/alireza.egg-info/PKG-INFO` & `alireza-0.0.3/alireza.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alireza
-Version: 0.0.2
+Version: 0.0.3
 Summary: Useful tools for python frameworks
 Home-page: UNKNOWN
 Author: Alireza Soroush
 Author-email: alirezasoroush@hotmail.com
 License: UNKNOWN
 Keywords: python,tools,framework,django
 Platform: UNKNOWN
```

### Comparing `alireza-0.0.2/setup.py` & `alireza-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Useful tools for python frameworks'
 LONG_DESCRIPTION = 'The purpose of starting this project is to make useful tools for all Python frameworks and make the life of programmers easier :)'
 
 # Setting up
 setup(
     name="alireza",
     version=VERSION,
```

