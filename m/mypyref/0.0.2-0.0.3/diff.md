# Comparing `tmp/mypyref-0.0.2.tar.gz` & `tmp/mypyref-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypyref-0.0.2.tar", last modified: Mon Jul  3 03:42:00 2023, max compression
+gzip compressed data, was "mypyref-0.0.3.tar", last modified: Mon Jul  3 04:27:20 2023, max compression
```

## Comparing `mypyref-0.0.2.tar` & `mypyref-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:42:00.661454 mypyref-0.0.2/
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-03 03:41:12.000000 mypyref-0.0.2/.version
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-03 03:42:00.661454 mypyref-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-03 03:41:52.000000 mypyref-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:42:00.659454 mypyref-0.0.2/mypyref/
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-03 03:41:52.000000 mypyref-0.0.2/mypyref/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-03 03:41:52.000000 mypyref-0.0.2/mypyref/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     2451 2023-07-03 03:41:52.000000 mypyref-0.0.2/mypyref/handler.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-03 03:41:52.000000 mypyref-0.0.2/mypyref/xbar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 03:42:00.660454 mypyref-0.0.2/mypyref.egg-info/
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-03 03:42:00.000000 mypyref-0.0.2/mypyref.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-03 03:42:00.000000 mypyref-0.0.2/mypyref.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 03:42:00.000000 mypyref-0.0.2/mypyref.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-03 03:42:00.000000 mypyref-0.0.2/mypyref.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-03 03:42:00.000000 mypyref-0.0.2/mypyref.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-03 03:41:52.000000 mypyref-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 03:42:00.661454 mypyref-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 04:27:20.793140 mypyref-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-03 04:26:32.000000 mypyref-0.0.3/.version
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-03 04:27:20.792140 mypyref-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-03 04:27:12.000000 mypyref-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 04:27:20.791140 mypyref-0.0.3/mypyref/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-03 04:27:12.000000 mypyref-0.0.3/mypyref/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-03 04:27:12.000000 mypyref-0.0.3/mypyref/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2451 2023-07-03 04:27:12.000000 mypyref-0.0.3/mypyref/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-03 04:27:12.000000 mypyref-0.0.3/mypyref/xbar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 04:27:20.792140 mypyref-0.0.3/mypyref.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-03 04:27:20.000000 mypyref-0.0.3/mypyref.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-03 04:27:20.000000 mypyref-0.0.3/mypyref.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 04:27:20.000000 mypyref-0.0.3/mypyref.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-03 04:27:20.000000 mypyref-0.0.3/mypyref.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-03 04:27:20.000000 mypyref-0.0.3/mypyref.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-07-03 04:27:12.000000 mypyref-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 04:27:20.793140 mypyref-0.0.3/setup.cfg
```

### Comparing `mypyref-0.0.2/mypyref/handler.py` & `mypyref-0.0.3/mypyref/handler.py`

 * *Files identical despite different names*

### Comparing `mypyref-0.0.2/pyproject.toml` & `mypyref-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mypyref"
 authors = [
-    {name = "Steampunk Wizard", email = "macdocpy@steampunkwizard.ca"}
+    {name = "Steampunk Wizard", email = "mypyrefcpy@steampunkwizard.ca"}
 ]
 description = "Standard Python reference documentation in a local server"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "MIT"}
 dependencies = [
     # "platformdirs >=3.2.0",
```

