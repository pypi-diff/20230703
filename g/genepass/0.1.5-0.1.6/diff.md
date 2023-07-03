# Comparing `tmp/genepass-0.1.5.tar.gz` & `tmp/genepass-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepass-0.1.5.tar", last modified: Fri Jun 23 14:11:19 2023, max compression
+gzip compressed data, was "genepass-0.1.6.tar", last modified: Mon Jul  3 03:50:47 2023, max compression
```

## Comparing `genepass-0.1.5.tar` & `genepass-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:11:19.874393 genepass-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 14:11:08.000000 genepass-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-23 14:11:19.874393 genepass-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-23 14:11:08.000000 genepass-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:11:19.874393 genepass-0.1.5/genepass/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 14:11:08.000000 genepass-0.1.5/genepass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-23 14:11:08.000000 genepass-0.1.5/genepass/genepass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:11:19.874393 genepass-0.1.5/genepass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-23 14:11:19.000000 genepass-0.1.5/genepass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-23 14:11:19.000000 genepass-0.1.5/genepass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:11:19.000000 genepass-0.1.5/genepass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 14:11:19.000000 genepass-0.1.5/genepass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:11:19.874393 genepass-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-23 14:11:08.000000 genepass-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:50:47.763654 genepass-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-03 03:50:34.000000 genepass-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-03 03:50:47.763654 genepass-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-03 03:50:34.000000 genepass-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:50:47.759654 genepass-0.1.6/genepass/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 03:50:34.000000 genepass-0.1.6/genepass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-03 03:50:34.000000 genepass-0.1.6/genepass/genepass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:50:47.763654 genepass-0.1.6/genepass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-03 03:50:47.000000 genepass-0.1.6/genepass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-03 03:50:47.000000 genepass-0.1.6/genepass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:50:47.000000 genepass-0.1.6/genepass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 03:50:47.000000 genepass-0.1.6/genepass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 03:50:47.763654 genepass-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 03:50:34.000000 genepass-0.1.6/setup.py
```

### Comparing `genepass-0.1.5/LICENSE` & `genepass-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `genepass-0.1.5/PKG-INFO` & `genepass-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: genepass
-Version: 0.1.5
-Summary: genepass can automatically generates passwords
+Version: 0.1.6
+Summary: genepass can automatically generate (create) passwords
 Home-page: https://github.com/senya-koku/genepass
 Author:  ny7777
-Author-email: meathouse47@gmail.com
+Author-email: 5938dai617@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # genepass
 
 generating passward randomly!
+（create password randomly）
 
 ----
 # Install
 `pip install genepass`
 
 ----
 # Usage
```

### Comparing `genepass-0.1.5/README.md` & `genepass-0.1.6/genepass.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,22 @@
+Metadata-Version: 2.1
+Name: genepass
+Version: 0.1.6
+Summary: genepass can automatically generate (create) passwords
+Home-page: https://github.com/senya-koku/genepass
+Author:  ny7777
+Author-email: 5938dai617@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # genepass
 
 generating passward randomly!
+（create password randomly）
 
 ----
 # Install
 `pip install genepass`
 
 ----
 # Usage
```

### Comparing `genepass-0.1.5/genepass/genepass.py` & `genepass-0.1.6/genepass/genepass.py`

 * *Files identical despite different names*

