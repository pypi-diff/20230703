# Comparing `tmp/segment-guard-0.0.1.tar.gz` & `tmp/segment-guard-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-guard-0.0.1.tar", last modified: Tue Jun 20 13:35:28 2023, max compression
+gzip compressed data, was "segment-guard-0.0.2.tar", last modified: Mon Jul  3 13:25:39 2023, max compression
```

## Comparing `segment-guard-0.0.1.tar` & `segment-guard-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-20 13:35:28.615208 segment-guard-0.0.1/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 segment-guard-0.0.1/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      817 2023-06-20 13:35:28.615208 segment-guard-0.0.1/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      151 2023-06-20 13:23:41.000000 segment-guard-0.0.1/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      716 2023-06-20 13:35:19.000000 segment-guard-0.0.1/pyproject.toml
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-20 13:35:28.615208 segment-guard-0.0.1/segment_guard/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-06-14 08:02:02.000000 segment-guard-0.0.1/segment_guard/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-06-20 13:35:28.615208 segment-guard-0.0.1/segment_guard.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      817 2023-06-20 13:35:28.000000 segment-guard-0.0.1/segment_guard.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      206 2023-06-20 13:35:28.000000 segment-guard-0.0.1/segment_guard.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-06-20 13:35:28.000000 segment-guard-0.0.1/segment_guard.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-06-20 13:35:28.000000 segment-guard-0.0.1/segment_guard.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-06-20 13:35:28.615208 segment-guard-0.0.1/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-03 13:25:39.256354 segment-guard-0.0.2/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1065 2023-06-14 07:59:41.000000 segment-guard-0.0.2/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      961 2023-07-03 13:25:39.256354 segment-guard-0.0.2/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      294 2023-07-03 11:27:11.000000 segment-guard-0.0.2/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1056 2023-07-03 11:32:23.000000 segment-guard-0.0.2/pyproject.toml
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-03 13:25:39.256354 segment-guard-0.0.2/segment_guard/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       52 2023-06-21 13:56:24.000000 segment-guard-0.0.2/segment_guard/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5828 2023-07-03 11:25:32.000000 segment-guard-0.0.2/segment_guard/detection.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     2517 2023-06-30 11:10:59.000000 segment-guard-0.0.2/segment_guard/embedding_utils.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4346 2023-07-03 11:25:32.000000 segment-guard-0.0.2/segment_guard/explanation.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     7979 2023-07-03 13:18:08.000000 segment-guard-0.0.2/segment_guard/segment_guard.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6830 2023-07-03 11:25:32.000000 segment-guard-0.0.2/segment_guard/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-03 13:25:39.256354 segment-guard-0.0.2/segment_guard.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      961 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      413 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      232 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-07-03 13:25:39.000000 segment-guard-0.0.2/segment_guard.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-03 13:25:39.256354 segment-guard-0.0.2/setup.cfg
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-03 13:25:39.256354 segment-guard-0.0.2/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4385 2023-07-03 11:25:32.000000 segment-guard-0.0.2/tests/test_segment_guard.py
```

### Comparing `segment-guard-0.0.1/LICENSE` & `segment-guard-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-guard-0.0.1/PKG-INFO` & `segment-guard-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: segment-guard
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for detecting critical data segments in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/segment-guard
 Project-URL: Bug Tracker, https://github.com/Renumics/segment-guard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # segment-guard
 A library for detecting critical data segments in structured and unstructured data based on features, metadata and model predictions.
 
+## For building the library
+Follow this description: [Packaging Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
```

### Comparing `segment-guard-0.0.1/segment_guard.egg-info/PKG-INFO` & `segment-guard-0.0.2/segment_guard.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: segment-guard
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for detecting critical data segments in structured and unstructured data based on features, metadata and model predictions.
 Author-email: Renumics GmbH <info@renumics.com>, Daniel Klitzke <daniel.klitzke@renumics.com>
 Project-URL: Homepage, https://github.com/Renumics/segment-guard
 Project-URL: Bug Tracker, https://github.com/Renumics/segment-guard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # segment-guard
 A library for detecting critical data segments in structured and unstructured data based on features, metadata and model predictions.
 
+## For building the library
+Follow this description: [Packaging Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
```

