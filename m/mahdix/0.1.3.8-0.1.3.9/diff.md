# Comparing `tmp/mahdix-0.1.3.8.tar.gz` & `tmp/mahdix-0.1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahdix-0.1.3.8.tar", last modified: Fri Jun 30 06:20:39 2023, max compression
+gzip compressed data, was "mahdix-0.1.3.9.tar", last modified: Mon Jul  3 18:07:09 2023, max compression
```

## Comparing `mahdix-0.1.3.8.tar` & `mahdix-0.1.3.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:20:39.935813 mahdix-0.1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-30 06:20:39.935813 mahdix-0.1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-30 06:20:25.000000 mahdix-0.1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:20:39.935813 mahdix-0.1.3.8/mahdix/
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-30 06:20:25.000000 mahdix-0.1.3.8/mahdix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 06:20:39.935813 mahdix-0.1.3.8/mahdix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-30 06:20:39.000000 mahdix-0.1.3.8/mahdix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-30 06:20:39.000000 mahdix-0.1.3.8/mahdix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 06:20:39.000000 mahdix-0.1.3.8/mahdix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 06:20:39.000000 mahdix-0.1.3.8/mahdix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 06:20:39.935813 mahdix-0.1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-30 06:20:25.000000 mahdix-0.1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:07:09.025851 mahdix-0.1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-03 18:07:09.025851 mahdix-0.1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 18:06:57.000000 mahdix-0.1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:07:09.021850 mahdix-0.1.3.9/mahdix/
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-07-03 18:06:57.000000 mahdix-0.1.3.9/mahdix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 18:07:09.025851 mahdix-0.1.3.9/mahdix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-03 18:07:09.000000 mahdix-0.1.3.9/mahdix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-03 18:07:09.000000 mahdix-0.1.3.9/mahdix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 18:07:09.000000 mahdix-0.1.3.9/mahdix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 18:07:09.000000 mahdix-0.1.3.9/mahdix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 18:07:09.025851 mahdix-0.1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-03 18:06:57.000000 mahdix-0.1.3.9/setup.py
```

### Comparing `mahdix-0.1.3.8/PKG-INFO` & `mahdix-0.1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahdix
-Version: 0.1.3.8
+Version: 0.1.3.9
 Summary: this is a simple pip modul and test
 
 
 # pip install mahdix
 
 # ----[USE]-------
```

### Comparing `mahdix-0.1.3.8/README.md` & `mahdix-0.1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mahdix-0.1.3.8/mahdix/__init__.py` & `mahdix-0.1.3.9/mahdix/__init__.py`

 * *Files identical despite different names*

### Comparing `mahdix-0.1.3.8/mahdix.egg-info/PKG-INFO` & `mahdix-0.1.3.9/mahdix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mahdix
-Version: 0.1.3.8
+Version: 0.1.3.9
 Summary: this is a simple pip modul and test
 
 
 # pip install mahdix
 
 # ----[USE]-------
```

### Comparing `mahdix-0.1.3.8/setup.py` & `mahdix-0.1.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='mahdix',
-version='0.1.3.8',
+version='0.1.3.9',
 description='this is a simple pip modul and test',
 long_description='''
 # pip install mahdix
 
 # ----[USE]-------
 
 # print Sumthiong = mahdix.p('YOUR TXT')
```

