# Comparing `tmp/devvit-manager-1.0.0.tar.gz` & `tmp/devvit-manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvit-manager-1.0.0.tar", last modified: Mon Jul  3 01:16:41 2023, max compression
+gzip compressed data, was "devvit-manager-1.0.1.tar", last modified: Mon Jul  3 01:29:49 2023, max compression
```

## Comparing `devvit-manager-1.0.0.tar` & `devvit-manager-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:16:41.638852 devvit-manager-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-03 01:16:41.638852 devvit-manager-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:16:41.638852 devvit-manager-1.0.0/devvit_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-03 01:16:41.000000 devvit-manager-1.0.0/devvit_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-03 01:16:41.000000 devvit-manager-1.0.0/devvit_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:16:41.000000 devvit-manager-1.0.0/devvit_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 01:16:41.000000 devvit-manager-1.0.0/devvit_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 01:16:41.000000 devvit-manager-1.0.0/devvit_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 01:16:41.000000 devvit-manager-1.0.0/devvit_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:16:41.638852 devvit-manager-1.0.0/devvit_mgr/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/devvit_mgr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/devvit_mgr/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/devvit_mgr/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/devvit_mgr/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/devvit_mgr/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 01:16:22.000000 devvit-manager-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-03 01:16:41.638852 devvit-manager-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:29:49.734580 devvit-manager-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-03 01:29:49.734580 devvit-manager-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:29:49.734580 devvit-manager-1.0.1/devvit_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-03 01:29:49.000000 devvit-manager-1.0.1/devvit_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-03 01:29:49.000000 devvit-manager-1.0.1/devvit_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:29:49.000000 devvit-manager-1.0.1/devvit_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 01:29:49.000000 devvit-manager-1.0.1/devvit_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 01:29:49.000000 devvit-manager-1.0.1/devvit_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 01:29:49.000000 devvit-manager-1.0.1/devvit_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:29:49.734580 devvit-manager-1.0.1/devvit_mgr/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/devvit_mgr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/devvit_mgr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/devvit_mgr/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/devvit_mgr/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/devvit_mgr/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 01:29:38.000000 devvit-manager-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-03 01:29:49.734580 devvit-manager-1.0.1/setup.cfg
```

### Comparing `devvit-manager-1.0.0/LICENSE.txt` & `devvit-manager-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devvit-manager-1.0.0/PKG-INFO` & `devvit-manager-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: devvit-manager
-Version: 1.0.0
-Summary: Devvit Manager is a Python package that enables you to easily utilize
+Version: 1.0.1
+Summary: Devvit Manager is a Python package that enables you to easily utilize devvit with multiple Reddit user accounts.
 Author: Joel Payne
 Author-email: lilspazjoekp@gmail.com
 License: Simplified BSD License
 Keywords: devvit manager reddit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `devvit-manager-1.0.0/README.rst` & `devvit-manager-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `devvit-manager-1.0.0/devvit_manager.egg-info/PKG-INFO` & `devvit-manager-1.0.1/devvit_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: devvit-manager
-Version: 1.0.0
-Summary: Devvit Manager is a Python package that enables you to easily utilize
+Version: 1.0.1
+Summary: Devvit Manager is a Python package that enables you to easily utilize devvit with multiple Reddit user accounts.
 Author: Joel Payne
 Author-email: lilspazjoekp@gmail.com
 License: Simplified BSD License
 Keywords: devvit manager reddit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `devvit-manager-1.0.0/devvit_mgr/cli.py` & `devvit-manager-1.0.1/devvit_mgr/cli.py`

 * *Files identical despite different names*

### Comparing `devvit-manager-1.0.0/devvit_mgr/manager.py` & `devvit-manager-1.0.1/devvit_mgr/manager.py`

 * *Files identical despite different names*

### Comparing `devvit-manager-1.0.0/devvit_mgr/models.py` & `devvit-manager-1.0.1/devvit_mgr/models.py`

 * *Files identical despite different names*

### Comparing `devvit-manager-1.0.0/setup.cfg` & `devvit-manager-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Utilities
-description = Devvit Manager is a Python package that enables you to easily utilize
-	devvit with multiple Reddit user accounts.
+description = Devvit Manager is a Python package that enables you to easily utilize devvit with multiple Reddit user accounts.
 keywords = devvit manager reddit
 license = Simplified BSD License
 long_description = file: README.rst
 name = devvit-manager
 version = attr: devvit_mgr.__version__
 
 [options]
```

