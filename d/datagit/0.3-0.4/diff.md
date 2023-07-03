# Comparing `tmp/datagit-0.3.tar.gz` & `tmp/datagit-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagit-0.3.tar", last modified: Thu Jun  1 09:44:05 2023, max compression
+gzip compressed data, was "datagit-0.4.tar", last modified: Mon Jul  3 14:36:36 2023, max compression
```

## Comparing `datagit-0.3.tar` & `datagit-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-01 09:44:05.697644 datagit-0.3/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3126 2023-06-01 09:44:05.697500 datagit-0.3/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)     2726 2023-06-01 09:39:55.000000 datagit-0.3/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-01 09:44:05.696351 datagit-0.3/datagit/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.3/datagit/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      635 2023-05-23 16:37:26.000000 datagit-0.3/datagit/dataset_helpers.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     4313 2023-05-23 16:37:26.000000 datagit-0.3/datagit/github_connector.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.3/datagit/query_builder.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-01 09:44:05.697256 datagit-0.3/datagit.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3126 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-06-01 09:44:05.000000 datagit-0.3/datagit.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-01 09:44:05.697697 datagit-0.3/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-06-01 09:41:42.000000 datagit-0.3/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 14:36:36.219774 datagit-0.4/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3126 2023-07-03 14:36:36.219642 datagit-0.4/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2726 2023-06-01 09:39:55.000000 datagit-0.4/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 14:36:36.218777 datagit-0.4/datagit/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-05-22 13:02:30.000000 datagit-0.4/datagit/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      635 2023-05-23 16:37:26.000000 datagit-0.4/datagit/dataset_helpers.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)    10181 2023-07-03 14:35:24.000000 datagit-0.4/datagit/github_connector.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-05-23 14:01:11.000000 datagit-0.4/datagit/query_builder.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-03 14:36:36.219442 datagit-0.4/datagit.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3126 2023-07-03 14:36:36.000000 datagit-0.4/datagit.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-07-03 14:36:36.000000 datagit-0.4/datagit.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-03 14:36:36.000000 datagit-0.4/datagit.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-07-03 14:36:36.000000 datagit-0.4/datagit.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-07-03 14:36:36.000000 datagit-0.4/datagit.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-03 14:36:36.219834 datagit-0.4/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-07-03 14:35:39.000000 datagit-0.4/setup.py
```

### Comparing `datagit-0.3/PKG-INFO` & `datagit-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.3
+Version: 0.4
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datagit-0.3/README.md` & `datagit-0.4/README.md`

 * *Files identical despite different names*

### Comparing `datagit-0.3/datagit/dataset_helpers.py` & `datagit-0.4/datagit/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `datagit-0.3/datagit/query_builder.py` & `datagit-0.4/datagit/query_builder.py`

 * *Files identical despite different names*

### Comparing `datagit-0.3/datagit.egg-info/PKG-INFO` & `datagit-0.4/datagit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.3
+Version: 0.4
 Summary: Git based metric store
 Home-page: https://github.com/data-drift/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datagit-0.3/setup.py` & `datagit-0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="datagit",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     author="Sammy Teillet",
     author_email="sammy.teillet@gmail.com",
     description="Git based metric store",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/data-drift/datagit",
```

