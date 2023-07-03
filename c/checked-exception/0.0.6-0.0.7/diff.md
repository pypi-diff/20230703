# Comparing `tmp/checked-exception-0.0.6.tar.gz` & `tmp/checked-exception-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checked-exception-0.0.6.tar", last modified: Wed Jun 28 09:08:29 2023, max compression
+gzip compressed data, was "checked-exception-0.0.7.tar", last modified: Mon Jul  3 08:25:04 2023, max compression
```

## Comparing `checked-exception-0.0.6.tar` & `checked-exception-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-06-28 09:08:29.129372 checked-exception-0.0.6/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-28 08:42:14.000000 checked-exception-0.0.6/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)      581 2023-06-28 09:08:29.129243 checked-exception-0.0.6/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)     1077 2023-06-28 09:02:48.000000 checked-exception-0.0.6/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-06-28 09:08:29.128478 checked-exception-0.0.6/checked_exception/
--rw-r--r--   0 j3ymac     (501) staff       (20)       83 2023-06-28 08:42:14.000000 checked-exception-0.0.6/checked_exception/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-06-28 09:08:29.129088 checked-exception-0.0.6/checked_exception.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)      581 2023-06-28 09:08:29.000000 checked-exception-0.0.6/checked_exception.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      220 2023-06-28 09:08:29.000000 checked-exception-0.0.6/checked_exception.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-06-28 09:08:29.000000 checked-exception-0.0.6/checked_exception.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       18 2023-06-28 09:08:29.000000 checked-exception-0.0.6/checked_exception.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-06-28 09:08:29.129411 checked-exception-0.0.6/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      719 2023-06-28 09:07:55.000000 checked-exception-0.0.6/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-03 08:25:04.032781 checked-exception-0.0.7/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-28 08:42:14.000000 checked-exception-0.0.7/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)      581 2023-07-03 08:25:04.032592 checked-exception-0.0.7/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1077 2023-06-28 09:02:48.000000 checked-exception-0.0.7/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-03 08:25:04.031487 checked-exception-0.0.7/checked_exception/
+-rw-r--r--   0 j3ymac     (501) staff       (20)       83 2023-06-28 08:42:14.000000 checked-exception-0.0.7/checked_exception/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-03 08:25:04.032307 checked-exception-0.0.7/checked_exception.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)      581 2023-07-03 08:25:04.000000 checked-exception-0.0.7/checked_exception.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      220 2023-07-03 08:25:04.000000 checked-exception-0.0.7/checked_exception.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-03 08:25:04.000000 checked-exception-0.0.7/checked_exception.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       18 2023-07-03 08:25:04.000000 checked-exception-0.0.7/checked_exception.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-03 08:25:04.032835 checked-exception-0.0.7/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      719 2023-07-03 08:23:24.000000 checked-exception-0.0.7/setup.py
```

### Comparing `checked-exception-0.0.6/LICENSE` & `checked-exception-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `checked-exception-0.0.6/PKG-INFO` & `checked-exception-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checked-exception
-Version: 0.0.6
+Version: 0.0.7
 Summary: Use checked exceptions in Python.
 Home-page: https://github.com/thejimmylin/checked-exception
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `checked-exception-0.0.6/README.md` & `checked-exception-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `checked-exception-0.0.6/checked_exception.egg-info/PKG-INFO` & `checked-exception-0.0.7/checked_exception.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checked-exception
-Version: 0.0.6
+Version: 0.0.7
 Summary: Use checked exceptions in Python.
 Home-page: https://github.com/thejimmylin/checked-exception
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `checked-exception-0.0.6/setup.py` & `checked-exception-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="checked-exception",
-    version="0.0.6",
+    version="0.0.7",
     author="thejimmylin",
     author_email="b00502013@gmail.com",
     description="Use checked exceptions in Python.",
     long_description=(
         "# Use checked exceptions in Python.\n"
         "\n"
         "This package makes you use checked exceptions in Python.\n"
```

