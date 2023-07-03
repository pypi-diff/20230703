# Comparing `tmp/pipelinewise-tap-s3-csv-3.0.0.tar.gz` & `tmp/pipelinewise-tap-s3-csv-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinewise-tap-s3-csv-3.0.0.tar", last modified: Fri Dec  2 11:58:18 2022, max compression
+gzip compressed data, was "pipelinewise-tap-s3-csv-3.0.1.tar", last modified: Mon Jul  3 15:43:21 2023, max compression
```

## Comparing `pipelinewise-tap-s3-csv-3.0.0.tar` & `pipelinewise-tap-s3-csv-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 11:58:18.006671 pipelinewise-tap-s3-csv-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    32393 2022-12-02 11:58:08.000000 pipelinewise-tap-s3-csv-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2022-12-02 11:58:18.006671 pipelinewise-tap-s3-csv-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2022-12-02 11:58:08.000000 pipelinewise-tap-s3-csv-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 11:58:18.006671 pipelinewise-tap-s3-csv-3.0.0/pipelinewise_tap_s3_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2022-12-02 11:58:17.000000 pipelinewise-tap-s3-csv-3.0.0/pipelinewise_tap_s3_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2022-12-02 11:58:17.000000 pipelinewise-tap-s3-csv-3.0.0/pipelinewise_tap_s3_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 11:58:17.000000 pipelinewise-tap-s3-csv-3.0.0/pipelinewise_tap_s3_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-02 11:58:17.000000 pipelinewise-tap-s3-csv-3.0.0/pipelinewise_tap_s3_csv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2022-12-02 11:58:17.000000 pipelinewise-tap-s3-csv-3.0.0/pipelinewise_tap_s3_csv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-02 11:58:17.000000 pipelinewise-tap-s3-csv-3.0.0/pipelinewise_tap_s3_csv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-02 11:58:18.006671 pipelinewise-tap-s3-csv-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2022-12-02 11:58:08.000000 pipelinewise-tap-s3-csv-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 11:58:18.006671 pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2022-12-02 11:58:08.000000 pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2022-12-02 11:58:08.000000 pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2022-12-02 11:58:08.000000 pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)    11478 2022-12-02 11:58:08.000000 pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2022-12-02 11:58:08.000000 pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:21.162410 pipelinewise-tap-s3-csv-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-07-03 15:43:12.000000 pipelinewise-tap-s3-csv-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-03 15:43:21.162410 pipelinewise-tap-s3-csv-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-03 15:43:12.000000 pipelinewise-tap-s3-csv-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:21.162410 pipelinewise-tap-s3-csv-3.0.1/pipelinewise_tap_s3_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-03 15:43:21.000000 pipelinewise-tap-s3-csv-3.0.1/pipelinewise_tap_s3_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 15:43:21.000000 pipelinewise-tap-s3-csv-3.0.1/pipelinewise_tap_s3_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:43:21.000000 pipelinewise-tap-s3-csv-3.0.1/pipelinewise_tap_s3_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 15:43:21.000000 pipelinewise-tap-s3-csv-3.0.1/pipelinewise_tap_s3_csv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 15:43:21.000000 pipelinewise-tap-s3-csv-3.0.1/pipelinewise_tap_s3_csv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 15:43:21.000000 pipelinewise-tap-s3-csv-3.0.1/pipelinewise_tap_s3_csv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:43:21.162410 pipelinewise-tap-s3-csv-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-03 15:43:12.000000 pipelinewise-tap-s3-csv-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:43:21.162410 pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-03 15:43:12.000000 pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-03 15:43:12.000000 pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-03 15:43:12.000000 pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-07-03 15:43:12.000000 pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-03 15:43:12.000000 pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/sync.py
```

### Comparing `pipelinewise-tap-s3-csv-3.0.0/LICENSE` & `pipelinewise-tap-s3-csv-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-s3-csv-3.0.0/PKG-INFO` & `pipelinewise-tap-s3-csv-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-s3-csv
-Version: 3.0.0
+Version: 3.0.1
 Summary: Singer.io tap for extracting CSV files from S3 - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-s3-csv
 Author: TransferWise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `pipelinewise-tap-s3-csv-3.0.0/README.md` & `pipelinewise-tap-s3-csv-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-s3-csv-3.0.0/pipelinewise_tap_s3_csv.egg-info/PKG-INFO` & `pipelinewise-tap-s3-csv-3.0.1/pipelinewise_tap_s3_csv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-s3-csv
-Version: 3.0.0
+Version: 3.0.1
 Summary: Singer.io tap for extracting CSV files from S3 - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-s3-csv
 Author: TransferWise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `pipelinewise-tap-s3-csv-3.0.0/setup.py` & `pipelinewise-tap-s3-csv-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='pipelinewise-tap-s3-csv',
-      version='3.0.0',
+      version='3.0.1',
       description='Singer.io tap for extracting CSV files from S3 - PipelineWise compatible',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='TransferWise',
       url='https://github.com/transferwise/pipelinewise-tap-s3-csv',
       classifiers=[
           'License :: OSI Approved :: GNU Affero General Public License v3',
           'Programming Language :: Python :: 3 :: Only'
       ],
       py_modules=['tap_s3_csv'],
       install_requires=[
-          'boto3==1.26.21',
+          'boto3==1.26.165',
           'singer-encodings==0.0.*',
           'pipelinewise-singer-python==1.*',
           'voluptuous==0.13.1',
           'ujson==5.4.0',
           'more_itertools==8.12.*',
       ],
       extras_require={
```

### Comparing `pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/__init__.py` & `pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/discover.py` & `pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/discover.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/s3.py` & `pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,20 +291,20 @@
         'MaxKeys': max_results,
     }
 
     if search_prefix is not None:
         args['Prefix'] = search_prefix
 
     paginator = s3_client.get_paginator('list_objects_v2')
-    pages = 0
-    for page in paginator.paginate(**args):
-        pages += 1
-        LOGGER.debug("On page %s", pages)
-        s3_object_count += len(page.get('Contents', []))
-        yield from page.get('Contents', [])
+    page_iterator = paginator.paginate(**args)
+    filtered_s3_objects = page_iterator.search("Contents[?StorageClass=='STANDARD']")
+
+    for s3_obj in filtered_s3_objects:
+        s3_object_count += 1
+        yield s3_obj
 
     if s3_object_count > 0:
         LOGGER.info("Found %s files.", s3_object_count)
     else:
         LOGGER.warning('Found no files for bucket "%s" that match prefix "%s"', bucket, search_prefix)
```

### Comparing `pipelinewise-tap-s3-csv-3.0.0/tap_s3_csv/sync.py` & `pipelinewise-tap-s3-csv-3.0.1/tap_s3_csv/sync.py`

 * *Files identical despite different names*

