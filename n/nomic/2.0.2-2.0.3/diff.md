# Comparing `tmp/nomic-2.0.2.tar.gz` & `tmp/nomic-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomic-2.0.2.tar", last modified: Thu Jun 29 14:13:59 2023, max compression
+gzip compressed data, was "nomic-2.0.3.tar", last modified: Mon Jul  3 15:01:21 2023, max compression
```

## Comparing `nomic-2.0.2.tar` & `nomic-2.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 14:13:59.949231 nomic-2.0.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2023-06-29 14:13:59.949231 nomic-2.0.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2023-06-29 14:13:52.000000 nomic-2.0.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 14:13:59.949231 nomic-2.0.2/nomic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10917 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/atlas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4531 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2040 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/data_inference.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27888 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/data_operations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2028 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/embedders.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 14:13:59.949231 nomic-2.0.2/nomic/pl_callbacks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/pl_callbacks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6975 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/pl_callbacks/pl_callback.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    57666 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/project.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      521 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 14:13:59.949231 nomic-2.0.2/nomic/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10483 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/tests/test_atlas_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1502 2023-06-29 14:13:52.000000 nomic-2.0.2/nomic/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 14:13:59.949231 nomic-2.0.2/nomic.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2023-06-29 14:13:59.000000 nomic-2.0.2/nomic.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2023-06-29 14:13:59.000000 nomic-2.0.2/nomic.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-29 14:13:59.000000 nomic-2.0.2/nomic.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-06-29 14:13:59.000000 nomic-2.0.2/nomic.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      223 2023-06-29 14:13:59.000000 nomic-2.0.2/nomic.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-06-29 14:13:59.000000 nomic-2.0.2/nomic.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-29 14:13:59.949231 nomic-2.0.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1259 2023-06-29 14:13:52.000000 nomic-2.0.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2023-07-03 15:01:21.990885 nomic-2.0.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2023-07-03 15:01:15.000000 nomic-2.0.3/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/nomic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10917 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/atlas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4531 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2040 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/data_inference.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28176 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/data_operations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2028 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/embedders.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/nomic/pl_callbacks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/pl_callbacks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6975 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/pl_callbacks/pl_callback.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    57993 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/project.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      521 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/nomic/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10483 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/tests/test_atlas_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1502 2023-07-03 15:01:15.000000 nomic-2.0.3/nomic/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 15:01:21.990885 nomic-2.0.3/nomic.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      223 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-07-03 15:01:21.000000 nomic-2.0.3/nomic.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-03 15:01:21.990885 nomic-2.0.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1259 2023-07-03 15:01:15.000000 nomic-2.0.3/setup.py
```

### Comparing `nomic-2.0.2/README.md` & `nomic-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nomic-2.0.2/nomic/atlas.py` & `nomic-2.0.3/nomic/atlas.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.2/nomic/cli.py` & `nomic-2.0.3/nomic/cli.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.2/nomic/data_inference.py` & `nomic-2.0.3/nomic/data_inference.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.2/nomic/data_operations.py` & `nomic-2.0.3/nomic/data_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,18 @@
         9999  JZU            singleton         6346
         ```
     """
 
     def __init__(self, projection: "AtlasProjection"):
         self.projection = projection
         self.id_field = self.projection.project.id_field
-        self._tb: pa.Table = projection._fetch_tiles().select([self.id_field, '_duplicate_class', '_cluster_id'])
+        try:
+            self._tb: pa.Table = projection._fetch_tiles().select([self.id_field, '_duplicate_class', '_cluster_id'])
+        except pa.lib.ArrowInvalid as e:
+            raise ValueError("Duplicate detection has not yet been run on this map.")
         self._tb = self._tb.rename_columns([self.id_field, 'duplicate_class', 'cluster_id'])
 
     @property
     def df(self) -> pd.DataFrame:
         """
         Pandas dataframe mapping each data point to its cluster of semantically similar points
 
@@ -95,23 +98,23 @@
 
     def deletion_candidates(self) -> List[str]:
         """
 
         Returns:
             The ids for all data points which are semantic duplicates and are candidates for being deleted from the dataset. If you remove these data points from your dataset, your dataset will be semantically deduplicated.
         """
-        dupes = self.tb[self.id_field].filter(pc.equal(self.tb['_duplicate_class'], 'deletion candidate'))
+        dupes = self.tb[self.id_field].filter(pc.equal(self.tb['duplicate_class'], 'deletion candidate'))
         return dupes.to_pylist()
 
     def __repr__(self) -> str:
         repr = f"===Atlas Duplicates for ({self.projection})===\n"
         duplicate_count = len(
-            self.tb[self.id_field].filter(pc.equal(self.tb['_duplicate_class'], 'deletion candidate'))
+            self.tb[self.id_field].filter(pc.equal(self.tb['duplicate_class'], 'deletion candidate'))
         )
-        cluster_count = len(self.tb['_cluster_id'].value_counts())
+        cluster_count = len(self.tb['cluster_id'].value_counts())
         repr += f"{duplicate_count} deletion candidates in {cluster_count} clusters\n"
         return repr + self.df.__repr__()
 
 
 class AtlasMapTopics:
     """
     Atlas Topics State
@@ -134,17 +137,20 @@
         ```
     """
 
     def __init__(self, projection: "AtlasProjection"):
         self.projection = projection
         self.project = projection.project
         self.id_field = self.projection.project.id_field
-        self._tb: pa.Table = projection._fetch_tiles().select(
-            [self.id_field, '_topic_depth_1', '_topic_depth_2', '_topic_depth_3']
-        ).rename_columns([self.id_field, 'topic_depth_1', 'topic_depth_2', 'topic_depth_3'])
+        try:
+            self._tb: pa.Table = projection._fetch_tiles().select(
+                [self.id_field, '_topic_depth_1', '_topic_depth_2', '_topic_depth_3']
+            ).rename_columns([self.id_field, 'topic_depth_1', 'topic_depth_2', 'topic_depth_3'])
+        except pa.lib.ArrowInvalid as e:
+            raise ValueError("Topic modeling has not yet been run on this map.")
         self._metadata = None
         self._hierarchy = None
 
     @property
     def df(self) -> pandas.DataFrame:
         """
         A pandas dataframe associating each datapoint on your map to their topics as each topic depth.
```

### Comparing `nomic-2.0.2/nomic/embedders.py` & `nomic-2.0.3/nomic/embedders.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.2/nomic/pl_callbacks/pl_callback.py` & `nomic-2.0.3/nomic/pl_callbacks/pl_callback.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.2/nomic/project.py` & `nomic-2.0.3/nomic/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,30 +465,34 @@
             <h3>Project: {self.name}</h3>
             {self._embed_html()}
             """
 
     @property
     def duplicates(self):
         """Duplicate detection state"""
+        if self.project.is_locked:
+            raise Exception('Project is locked! Please wait until the project is unlocked to access duplicates.')
         if self._duplicates is None:
             self._duplicates = AtlasMapDuplicates(self)
         return self._duplicates
 
     @property
     def topics(self):
         """Topic state"""
         if self.project.is_locked:
-            raise Exception('Project is locked! Please wait until the project is unlocked to download embeddings')
+            raise Exception('Project is locked for state access! Please wait until the project is unlocked to access topics.')
         if self._topics is None:
             self._topics = AtlasMapTopics(self)
         return self._topics
 
     @property
     def embeddings(self):
         """Embedding state"""
+        if self.project.is_locked:
+            raise Exception('Project is locked for state access! Please wait until the project is unlocked to access embeddings.')
         if self._embeddings is None:
             self._embeddings = AtlasMapEmbeddings(self)
         return self._embeddings
 
     @property
     def tags(self):
         """Embedding state"""
```

### Comparing `nomic-2.0.2/nomic/settings.py` & `nomic-2.0.3/nomic/settings.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.2/nomic/tests/test_atlas_client.py` & `nomic-2.0.3/nomic/tests/test_atlas_client.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.2/nomic/utils.py` & `nomic-2.0.3/nomic/utils.py`

 * *Files identical despite different names*

### Comparing `nomic-2.0.2/setup.py` & `nomic-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 description = 'The official Nomic python client.'
     
 setup(
     name='nomic',
-    version='2.0.2',
+    version='2.0.3',
     url='https://github.com/nomic-ai/nomic',
     description=description,
     long_description=description,
     packages=find_packages(),
     author_email="support@nomic.ai",
     author="nomic.ai",
     classifiers=[
```

