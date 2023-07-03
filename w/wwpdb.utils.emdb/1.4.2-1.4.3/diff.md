# Comparing `tmp/wwpdb.utils.emdb-1.4.2.tar.gz` & `tmp/wwpdb.utils.emdb-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.emdb-1.4.2.tar", last modified: Thu Jun 29 15:14:17 2023, max compression
+gzip compressed data, was "wwpdb.utils.emdb-1.4.3.tar", last modified: Mon Jul  3 15:25:41 2023, max compression
```

## Comparing `wwpdb.utils.emdb-1.4.2.tar` & `wwpdb.utils.emdb-1.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 15:14:17.258762 wwpdb.utils.emdb-1.4.2/
--rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-06-29 15:14:17.258762 wwpdb.utils.emdb-1.4.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-29 15:14:17.258762 wwpdb.utils.emdb-1.4.2/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2278 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 15:14:17.250762 wwpdb.utils.emdb-1.4.2/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 15:14:17.250762 wwpdb.utils.emdb-1.4.2/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 15:14:17.250762 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (123)      145 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 15:14:17.254762 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/atomcheck/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/atomcheck/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11264 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/atomcheck/atomcheck.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 15:14:17.258762 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)   667797 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (123)  2283184 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)      389 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 15:14:17.258762 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (123)   217727 2023-06-29 15:13:21.000000 wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 15:14:17.250762 wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-06-29 15:14:17.000000 wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      975 2023-06-29 15:14:17.000000 wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-29 15:14:17.000000 wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-06-29 15:14:17.000000 wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-29 15:13:58.000000 wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-06-29 15:14:17.000000 wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-29 15:14:17.000000 wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/
+-rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2278 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.661876 wwpdb.utils.emdb-1.4.3/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.665876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.665876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      145 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.665876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/atomcheck/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/atomcheck/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7031 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/atomcheck/atomcheck.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   667797 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  2283184 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      389 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.669876 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)   217727 2023-07-03 15:24:44.000000 wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-03 15:25:41.665876 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      975 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-03 15:25:21.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-03 15:25:41.000000 wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.emdb-1.4.2/PKG-INFO` & `wwpdb.utils.emdb-1.4.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.4.2
+Version: 1.4.3
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.4.2/setup.py` & `wwpdb.utils.emdb-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py` & `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.2/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.4.3/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.4.2
+Version: 1.4.3
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.4.2/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb.utils.emdb-1.4.3/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

