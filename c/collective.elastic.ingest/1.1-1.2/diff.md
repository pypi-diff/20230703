# Comparing `tmp/collective.elastic.ingest-1.1.tar.gz` & `tmp/collective.elastic.ingest-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.elastic.ingest-1.1.tar", last modified: Fri Mar  3 12:05:43 2023, max compression
+gzip compressed data, was "collective.elastic.ingest-1.2.tar", last modified: Mon Jul  3 10:06:02 2023, max compression
```

## Comparing `collective.elastic.ingest-1.1.tar` & `collective.elastic.ingest-1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-03 12:05:43.633930 collective.elastic.ingest-1.1/
--rw-r--r--   0 katjasuss   (501) staff       (20)      359 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/CHANGES.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)       98 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/CONTRIBUTORS.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)    18092 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/LICENSE.GPL
--rw-r--r--   0 katjasuss   (501) staff       (20)      668 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/LICENSE.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)       56 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/MANIFEST.in
--rw-r--r--   0 katjasuss   (501) staff       (20)     6769 2023-03-03 12:05:43.634233 collective.elastic.ingest-1.1/PKG-INFO
--rw-r--r--   0 katjasuss   (501) staff       (20)     5241 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/README.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)      366 2023-03-03 12:05:43.634896 collective.elastic.ingest-1.1/setup.cfg
--rw-r--r--   0 katjasuss   (501) staff       (20)     1724 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/setup.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-03 12:05:43.623055 collective.elastic.ingest-1.1/src/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-03 12:05:43.626090 collective.elastic.ingest-1.1/src/collective/
--rw-r--r--   0 katjasuss   (501) staff       (20)       80 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/__init__.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-03 12:05:43.628184 collective.elastic.ingest-1.1/src/collective/elastic/
--rw-r--r--   0 katjasuss   (501) staff       (20)       80 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/__init__.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-03 12:05:43.631598 collective.elastic.ingest-1.1/src/collective/elastic/ingest/
--rw-r--r--   0 katjasuss   (501) staff       (20)      214 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/__init__.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-03 12:05:43.632698 collective.elastic.ingest-1.1/src/collective/elastic/ingest/analysis/
--rw-r--r--   0 katjasuss   (501) staff       (20)       38 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/analysis/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      738 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/analysis/analysis.json.example
--rw-r--r--   0 katjasuss   (501) staff       (20)     1740 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/analysis/analysis.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      289 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/analysis/elasticsearch-lexicon.txt.example
--rw-r--r--   0 katjasuss   (501) staff       (20)     2198 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/celery.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      805 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/elastic.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-03 12:05:43.633722 collective.elastic.ingest-1.1/src/collective/elastic/ingest/ingest/
--rw-r--r--   0 katjasuss   (501) staff       (20)     3094 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/ingest/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      366 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/ingest/section.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      207 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/ingest/security.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      801 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/ingest/vocabularyfields.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      328 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/logging.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     7005 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/mapping.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     6727 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/mappings.json
--rw-r--r--   0 katjasuss   (501) staff       (20)     2986 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/plone.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      928 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/postprocessing.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     6867 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/postprocessing_test.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     3723 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/preprocessing.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1641 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/preprocessing_test.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     2710 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/preprocessings.json
--rw-r--r--   0 katjasuss   (501) staff       (20)      500 2023-03-03 12:05:41.000000 collective.elastic.ingest-1.1/src/collective/elastic/ingest/removal.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-03-03 12:05:43.627927 collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/
--rw-r--r--   0 katjasuss   (501) staff       (20)     6769 2023-03-03 12:05:43.000000 collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/PKG-INFO
--rw-r--r--   0 katjasuss   (501) staff       (20)     1552 2023-03-03 12:05:43.000000 collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/SOURCES.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-03-03 12:05:43.000000 collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/dependency_links.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)       30 2023-03-03 12:05:43.000000 collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/namespace_packages.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-03-03 12:05:43.000000 collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/not-zip-safe
--rw-r--r--   0 katjasuss   (501) staff       (20)       61 2023-03-03 12:05:43.000000 collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/requires.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)       11 2023-03-03 12:05:43.000000 collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/top_level.txt
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-03 10:06:02.370137 collective.elastic.ingest-1.2/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      541 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/CHANGES.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)       98 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/CONTRIBUTORS.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)    18092 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/LICENSE.GPL
+-rw-r--r--   0 katjasuss   (501) staff       (20)      668 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/LICENSE.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)       56 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/MANIFEST.in
+-rw-r--r--   0 katjasuss   (501) staff       (20)     6951 2023-07-03 10:06:02.370261 collective.elastic.ingest-1.2/PKG-INFO
+-rw-r--r--   0 katjasuss   (501) staff       (20)     5241 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/README.rst
+-rw-r--r--   0 katjasuss   (501) staff       (20)      366 2023-07-03 10:06:02.370962 collective.elastic.ingest-1.2/setup.cfg
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1724 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/setup.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-03 10:06:02.360755 collective.elastic.ingest-1.2/src/
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-03 10:06:02.363418 collective.elastic.ingest-1.2/src/collective/
+-rw-r--r--   0 katjasuss   (501) staff       (20)       80 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-03 10:06:02.365280 collective.elastic.ingest-1.2/src/collective/elastic/
+-rw-r--r--   0 katjasuss   (501) staff       (20)       80 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-03 10:06:02.368177 collective.elastic.ingest-1.2/src/collective/elastic/ingest/
+-rw-r--r--   0 katjasuss   (501) staff       (20)      214 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/__init__.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-03 10:06:02.369075 collective.elastic.ingest-1.2/src/collective/elastic/ingest/analysis/
+-rw-r--r--   0 katjasuss   (501) staff       (20)       38 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/analysis/__init__.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      738 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/analysis/analysis.json.example
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1740 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/analysis/analysis.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      289 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/analysis/elasticsearch-lexicon.txt.example
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2198 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/celery.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      805 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/elastic.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-03 10:06:02.369958 collective.elastic.ingest-1.2/src/collective/elastic/ingest/ingest/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     3094 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/ingest/__init__.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      408 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/ingest/section.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      207 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/ingest/security.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      801 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/ingest/vocabularyfields.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      328 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/logging.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     7005 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/mapping.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     6727 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/mappings.json
+-rw-r--r--   0 katjasuss   (501) staff       (20)     2986 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/plone.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)      928 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/postprocessing.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     6867 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/postprocessing_test.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     3723 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/preprocessing.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1641 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/preprocessing_test.py
+-rw-r--r--   0 katjasuss   (501) staff       (20)     3003 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/preprocessings.json
+-rw-r--r--   0 katjasuss   (501) staff       (20)      500 2023-07-03 10:06:00.000000 collective.elastic.ingest-1.2/src/collective/elastic/ingest/removal.py
+drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2023-07-03 10:06:02.365017 collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/
+-rw-r--r--   0 katjasuss   (501) staff       (20)     6951 2023-07-03 10:06:02.000000 collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/PKG-INFO
+-rw-r--r--   0 katjasuss   (501) staff       (20)     1552 2023-07-03 10:06:02.000000 collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-07-03 10:06:02.000000 collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)       30 2023-07-03 10:06:02.000000 collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/namespace_packages.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)        1 2023-07-03 10:06:02.000000 collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/not-zip-safe
+-rw-r--r--   0 katjasuss   (501) staff       (20)       61 2023-07-03 10:06:02.000000 collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/requires.txt
+-rw-r--r--   0 katjasuss   (501) staff       (20)       11 2023-07-03 10:06:02.000000 collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/top_level.txt
```

### Comparing `collective.elastic.ingest-1.1/LICENSE.GPL` & `collective.elastic.ingest-1.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/LICENSE.rst` & `collective.elastic.ingest-1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/PKG-INFO` & `collective.elastic.ingest-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.elastic.ingest
-Version: 1.1
+Version: 1.2
 Summary: Addon for ElasticSearch integration with Plone
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.elastic.ingest
 Project-URL: Source, https://github.com/collective/collective.elastic.ingest
 Project-URL: Tracker, https://github.com/collective/collective.elastic.ingest/issues
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
@@ -73,19 +73,19 @@
     ANALYSIS_FILE=/full/path/to/analysis.json
     MAPPINGS_FILE=/full/path/to/mappings.json
     PREPROCESSINGS_FILE=/full/path/to/preprocessings.json
     SENTRY_DSN= (disabled by default)
 
 Then run celery::
 
-    celery worker -A collective.elastic.ingest.celery.app -l info
+    celery -A collective.elastic.ingest.celery.app worker -l info
 
 Or with debug information::
 
-    celery worker -A collective.elastic.ingest.celery.app -l debug
+    celery -A collective.elastic.ingest.celery.app worker -l debug
 
 
 Text Analysis
 -------------
 
 Test analysis is optional. Skip this on a first installation.
 
@@ -187,14 +187,22 @@
 The project is licensed under the GPLv2.
 
 
 Changelog
 =========
 
 
+1.2 (2023-07-03)
+----------------
+
+- Update example of preprocessing.json [ksuess]
+- Update README.rst: instruction on how to start celery [ksuess]
+- Add fallback section [ksuess]
+
+
 1.1 (2023-03-03)
 ----------------
 
 - Index allowedRolesAndUsers and section (primary path) [ksuess]
 
 
 1.0 (2022-11-08)
```

### Comparing `collective.elastic.ingest-1.1/README.rst` & `collective.elastic.ingest-1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -48,19 +48,19 @@
     ANALYSIS_FILE=/full/path/to/analysis.json
     MAPPINGS_FILE=/full/path/to/mappings.json
     PREPROCESSINGS_FILE=/full/path/to/preprocessings.json
     SENTRY_DSN= (disabled by default)
 
 Then run celery::
 
-    celery worker -A collective.elastic.ingest.celery.app -l info
+    celery -A collective.elastic.ingest.celery.app worker -l info
 
 Or with debug information::
 
-    celery worker -A collective.elastic.ingest.celery.app -l debug
+    celery -A collective.elastic.ingest.celery.app worker -l debug
 
 
 Text Analysis
 -------------
 
 Test analysis is optional. Skip this on a first installation.
```

### Comparing `collective.elastic.ingest-1.1/setup.py` & `collective.elastic.ingest-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     open('CHANGES.rst').read(),
     open('CONTRIBUTORS.rst').read(),
 ])
 
 
 setup(
     name="collective.elastic.ingest",
-    version="1.1",
+    version="1.2",
     project_urls={
         "PyPI": "https://pypi.python.org/pypi/collective.elastic.ingest",
         "Source": "https://github.com/collective/collective.elastic.ingest",
         "Tracker": "https://github.com/collective/collective.elastic.ingest/issues",
     },
     description="Addon for ElasticSearch integration with Plone",
     long_description=long_description,
```

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/analysis/analysis.json.example` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/analysis/analysis.json.example`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/analysis/analysis.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/celery.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/celery.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/elastic.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/elastic.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/ingest/__init__.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/ingest/vocabularyfields.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/ingest/vocabularyfields.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/mapping.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/mapping.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/mappings.json` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/mappings.json`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/plone.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/plone.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/postprocessing.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/postprocessing.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/postprocessing_test.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/postprocessing_test.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/preprocessing.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/preprocessing.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/preprocessing_test.py` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-1.1/src/collective/elastic/ingest/preprocessings.json` & `collective.elastic.ingest-1.2/src/collective/elastic/ingest/preprocessings.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.884920634920635%*

 * *Differences: {'10': "{'configuration': {'target': 'next_item'}}",*

 * * '6': "{'configuration': {'target': '@components'}}",*

 * * '7': "{'configuration': {'target': 'items'}}",*

 * * '8': "{'configuration': {'target': 'items_total'}}",*

 * * '9': "{'configuration': {'target': 'previous_item'}}",*

 * * 'insert': "[(0, OrderedDict([('match', OrderedDict([('type', 'always')])), ('action', 'remove'), "*

 * *           "('configuration', OrderedDict([('target', 'blocks')]))])), (1, OrderedDict([('match', "*

 * *           "OrderedDict([('type', 'always')])), […]*

```diff
@@ -1,9 +1,27 @@
 [
     {
+        "action": "remove",
+        "configuration": {
+            "target": "blocks"
+        },
+        "match": {
+            "type": "always"
+        }
+    },
+    {
+        "action": "remove",
+        "configuration": {
+            "target": "blocks_layout"
+        },
+        "match": {
+            "type": "always"
+        }
+    },
+    {
         "action": "additional_schema",
         "configuration": {
             "field": "zope.schema._field.ASCIILine",
             "name": "rid"
         },
         "match": {
             "type": "always"
@@ -39,51 +57,51 @@
         "match": {
             "type": "always"
         }
     },
     {
         "action": "remove",
         "configuration": {
-            "target": "@component"
+            "target": "@components"
         },
         "match": {
             "type": "always"
         }
     },
     {
         "action": "remove",
         "configuration": {
-            "target": "@id"
+            "target": "items"
         },
         "match": {
             "type": "always"
         }
     },
     {
         "action": "remove",
         "configuration": {
-            "target": "items"
+            "target": "items_total"
         },
         "match": {
             "type": "always"
         }
     },
     {
         "action": "remove",
         "configuration": {
-            "target": "items_total"
+            "target": "previous_item"
         },
         "match": {
             "type": "always"
         }
     },
     {
         "action": "remove",
         "configuration": {
-            "target": "parents"
+            "target": "next_item"
         },
         "match": {
             "type": "always"
         }
     },
     {
         "action": "remove",
```

### Comparing `collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/PKG-INFO` & `collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.elastic.ingest
-Version: 1.1
+Version: 1.2
 Summary: Addon for ElasticSearch integration with Plone
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.elastic.ingest
 Project-URL: Source, https://github.com/collective/collective.elastic.ingest
 Project-URL: Tracker, https://github.com/collective/collective.elastic.ingest/issues
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
@@ -73,19 +73,19 @@
     ANALYSIS_FILE=/full/path/to/analysis.json
     MAPPINGS_FILE=/full/path/to/mappings.json
     PREPROCESSINGS_FILE=/full/path/to/preprocessings.json
     SENTRY_DSN= (disabled by default)
 
 Then run celery::
 
-    celery worker -A collective.elastic.ingest.celery.app -l info
+    celery -A collective.elastic.ingest.celery.app worker -l info
 
 Or with debug information::
 
-    celery worker -A collective.elastic.ingest.celery.app -l debug
+    celery -A collective.elastic.ingest.celery.app worker -l debug
 
 
 Text Analysis
 -------------
 
 Test analysis is optional. Skip this on a first installation.
 
@@ -187,14 +187,22 @@
 The project is licensed under the GPLv2.
 
 
 Changelog
 =========
 
 
+1.2 (2023-07-03)
+----------------
+
+- Update example of preprocessing.json [ksuess]
+- Update README.rst: instruction on how to start celery [ksuess]
+- Add fallback section [ksuess]
+
+
 1.1 (2023-03-03)
 ----------------
 
 - Index allowedRolesAndUsers and section (primary path) [ksuess]
 
 
 1.0 (2022-11-08)
```

### Comparing `collective.elastic.ingest-1.1/src/collective.elastic.ingest.egg-info/SOURCES.txt` & `collective.elastic.ingest-1.2/src/collective.elastic.ingest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

