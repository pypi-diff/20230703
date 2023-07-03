# Comparing `tmp/nerdcore-0.0.0.tar.gz` & `tmp/nerdcore-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nerdcore-0.0.0.tar", last modified: Mon Jul  3 20:54:41 2023, max compression
+gzip compressed data, was "dist/nerdcore-0.0.1.tar", last modified: Mon Jul  3 20:59:38 2023, max compression
```

## Comparing `nerdcore-0.0.0.tar` & `nerdcore-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:54:41.000000 nerdcore-0.0.0/
--rw-r--r--   0 root         (0) root         (0)      848 2023-07-03 20:54:41.000000 nerdcore-0.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 20:54:22.000000 nerdcore-0.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:54:41.000000 nerdcore-0.0.0/nerdcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      848 2023-07-03 20:54:41.000000 nerdcore-0.0.0/nerdcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-03 20:54:41.000000 nerdcore-0.0.0/nerdcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:54:41.000000 nerdcore-0.0.0/nerdcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-03 20:54:41.000000 nerdcore-0.0.0/nerdcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 20:54:41.000000 nerdcore-0.0.0/nerdcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:54:41.000000 nerdcore-0.0.0/nerdcore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:54:41.000000 nerdcore-0.0.0/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2903 2023-07-03 20:54:22.000000 nerdcore-0.0.0/scripts/nerd
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-07-03 20:54:22.000000 nerdcore-0.0.0/scripts/nerd-new
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 20:54:41.000000 nerdcore-0.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 20:54:22.000000 nerdcore-0.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:59:38.000000 nerdcore-0.0.1/
+-rw-r--r--   0 root         (0) root         (0)      848 2023-07-03 20:59:38.000000 nerdcore-0.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 20:59:14.000000 nerdcore-0.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:59:38.000000 nerdcore-0.0.1/nerdcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      848 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:59:37.000000 nerdcore-0.0.1/nerdcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:59:38.000000 nerdcore-0.0.1/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2903 2023-07-03 20:59:14.000000 nerdcore-0.0.1/scripts/nerd
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-07-03 20:59:14.000000 nerdcore-0.0.1/scripts/nerd-new
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 20:59:38.000000 nerdcore-0.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-07-03 20:59:14.000000 nerdcore-0.0.1/setup.py
```

### Comparing `nerdcore-0.0.0/PKG-INFO` & `nerdcore-0.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.0.0
+Version: 0.0.1
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 License: UNKNOWN
-Description: # Nerdcore 🐵
+Description: # nerdcore 🤖
         
         Nerdcore is a package containing the core functionality used for the Nerd CLI.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.0.0/nerdcore.egg-info/PKG-INFO` & `nerdcore-0.0.1/nerdcore.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: nerdcore
-Version: 0.0.0
+Version: 0.0.1
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/fivable/nerd-cli.git
 Author: David Wallace Cooley Jr
 Author-email: david@fivable.com
 License: UNKNOWN
-Description: # Nerdcore 🐵
+Description: # nerdcore 🤖
         
         Nerdcore is a package containing the core functionality used for the Nerd CLI.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `nerdcore-0.0.0/scripts/nerd` & `nerdcore-0.0.1/scripts/nerd`

 * *Files identical despite different names*

### Comparing `nerdcore-0.0.0/scripts/nerd-new` & `nerdcore-0.0.1/scripts/nerd-new`

 * *Files identical despite different names*

### Comparing `nerdcore-0.0.0/setup.py` & `nerdcore-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nerdcore',
-    version='0.0.0',
+    version='0.0.1',
     __description__="Nerd CLI is a Fivable-specific and highly configurable CLI tool for creating/running deployments, " \
                     "commands, and more.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/fivable/nerd-cli.git',
     author='David Wallace Cooley Jr',
     author_email='david@fivable.com',
```

