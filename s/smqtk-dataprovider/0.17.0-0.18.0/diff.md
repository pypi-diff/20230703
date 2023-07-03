# Comparing `tmp/smqtk_dataprovider-0.17.0.tar.gz` & `tmp/smqtk_dataprovider-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smqtk_dataprovider-0.17.0.tar", max compression
+gzip compressed data, was "smqtk_dataprovider-0.18.0.tar", max compression
```

## Comparing `smqtk_dataprovider-0.17.0.tar` & `smqtk_dataprovider-0.18.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     1481 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/LICENSE.txt
--rw-r--r--   0        0        0      475 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/README.md
--rw-r--r--   0        0        0     4732 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/pyproject.toml
--rw-r--r--   0        0        0      268 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/__init__.py
--rw-r--r--   0        0        0     2838 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/content_type_validator.py
--rw-r--r--   0        0        0      569 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/exceptions.py
--rw-r--r--   0        0        0        0 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/__init__.py
--rw-r--r--   0        0        0        0 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/__init__.py
--rw-r--r--   0        0        0     7608 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/file.py
--rw-r--r--   0        0        0     8338 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/girder.py
--rw-r--r--   0        0        0     3957 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/hbase.py
--rw-r--r--   0        0        0     6092 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/matrix.py
--rw-r--r--   0        0        0     7451 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/memory.py
--rw-r--r--   0        0        0    16404 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/psql.py
--rw-r--r--   0        0        0     3426 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/url.py
--rw-r--r--   0        0        0        0 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_set/__init__.py
--rw-r--r--   0        0        0     8974 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_set/file.py
--rw-r--r--   0        0        0     5350 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_set/kvstore_backed.py
--rw-r--r--   0        0        0     8444 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_set/memory.py
--rw-r--r--   0        0        0    11832 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_set/psql.py
--rw-r--r--   0        0        0        0 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/key_value_store/__init__.py
--rw-r--r--   0        0        0    10180 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/key_value_store/memory.py
--rw-r--r--   0        0        0    21749 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/key_value_store/postgres.py
--rw-r--r--   0        0        0        0 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/interfaces/__init__.py
--rw-r--r--   0        0        0    11465 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/interfaces/data_element.py
--rw-r--r--   0        0        0     3264 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/interfaces/data_set.py
--rw-r--r--   0        0        0     7842 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/interfaces/key_value_store.py
--rw-r--r--   0        0        0        0 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/py.typed
--rw-r--r--   0        0        0       52 2022-12-13 00:01:46.193047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/utils/__init__.py
--rw-r--r--   0        0        0     9563 2022-12-13 00:01:46.197047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/utils/file.py
--rw-r--r--   0        0        0    16674 2022-12-13 00:01:46.197047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/utils/postgres.py
--rw-r--r--   0        0        0     1423 2022-12-13 00:01:46.197047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/utils/simple_timer.py
--rw-r--r--   0        0        0     3306 2022-12-13 00:01:46.197047 smqtk_dataprovider-0.17.0/smqtk_dataprovider/utils/string.py
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 smqtk_dataprovider-0.17.0/setup.py
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 smqtk_dataprovider-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0     1481 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/LICENSE.txt
+-rw-r--r--   0        0        0      475 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/README.md
+-rw-r--r--   0        0        0     4562 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/pyproject.toml
+-rw-r--r--   0        0        0      268 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/__init__.py
+-rw-r--r--   0        0        0     2838 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/content_type_validator.py
+-rw-r--r--   0        0        0      569 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/__init__.py
+-rw-r--r--   0        0        0     7608 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/file.py
+-rw-r--r--   0        0        0     8338 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/girder.py
+-rw-r--r--   0        0        0     3957 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/hbase.py
+-rw-r--r--   0        0        0     6092 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/matrix.py
+-rw-r--r--   0        0        0     7451 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/memory.py
+-rw-r--r--   0        0        0    16404 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/psql.py
+-rw-r--r--   0        0        0     3426 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/url.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_set/__init__.py
+-rw-r--r--   0        0        0     8974 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_set/file.py
+-rw-r--r--   0        0        0     5350 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_set/kvstore_backed.py
+-rw-r--r--   0        0        0     8444 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_set/memory.py
+-rw-r--r--   0        0        0    11832 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_set/psql.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/key_value_store/__init__.py
+-rw-r--r--   0        0        0    10180 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/key_value_store/memory.py
+-rw-r--r--   0        0        0    21749 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/key_value_store/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/interfaces/__init__.py
+-rw-r--r--   0        0        0    11465 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/interfaces/data_element.py
+-rw-r--r--   0        0        0     3264 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/interfaces/data_set.py
+-rw-r--r--   0        0        0     7842 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/interfaces/key_value_store.py
+-rw-r--r--   0        0        0        0 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/py.typed
+-rw-r--r--   0        0        0       52 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/utils/__init__.py
+-rw-r--r--   0        0        0     9563 2023-07-03 17:12:12.689730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/utils/file.py
+-rw-r--r--   0        0        0    16674 2023-07-03 17:12:12.693730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/utils/postgres.py
+-rw-r--r--   0        0        0     1423 2023-07-03 17:12:12.693730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/utils/simple_timer.py
+-rw-r--r--   0        0        0     3306 2023-07-03 17:12:12.693730 smqtk_dataprovider-0.18.0/smqtk_dataprovider/utils/string.py
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 smqtk_dataprovider-0.18.0/PKG-INFO
```

### Comparing `smqtk_dataprovider-0.17.0/LICENSE.txt` & `smqtk_dataprovider-0.18.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/pyproject.toml` & `smqtk_dataprovider-0.18.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,46 +4,43 @@
 
 ###############################################################################
 [tool.poetry]
 name = "smqtk_dataprovider"
 # REMEMBER: `distutils.version.*Version` types can be used to compare versions
 # from strings like this.
 # SMQTK prefers to use the strict numbering standard when possible.
-version = "0.17.0"
+version = "0.18.0"
 description = "SMQTK Data provision abstractions and implementations"
 license = "BSD-3-Clause"
 authors = ["Kitware, Inc. <smqtk-developers@kitware.com>"]
 readme = "README.md"
 repository = "https://github.com/Kitware/SMQTK-Dataprovider"
 documentation = "https://smqtk-dataprovider.readthedocs.io/"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Unix',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-numpy = [
-    { version = ">=1.21.1", python = "<3.8" },
-    { version = ">=1.23.5", python = ">=3.8" }
-]
+python = "^3.8"
+numpy = ">=1.23.5"
 requests = ">=2.28.1"
 smqtk-core = ">=0.19"
-girder-client = {version = "^3.1.3", optional = true}
-file-magic = {version = "^0.4.0", optional = true}
-psycopg2-binary = {version = "^2.9.5", optional = true}
+girder-client = {version = ">=3.1.3", optional = true}
+file-magic = {version = ">=0.4.0", optional = true}
+psycopg2-binary = {version = ">=2.9.5", optional = true}
 
 [tool.poetry.extras]
 girder = ["girder-client"]
 filemagic = ["file-magic"]
 psql = ["psycopg2-binary"]
 
 [tool.poetry.dev-dependencies]
@@ -71,18 +68,15 @@
 sphinx-prompt = ">=1.5"
 livereload = ">=2.6.3"
 # Testing
 coverage = ">=6.5"
 pytest = ">=7.2"
 pytest-cov = ">=4"
 # Development
-ipython = [
-    { version = ">=7.34.0", python = "<3.8" },
-    { version = ">=8.6.0", python = ">=3.8" }
-]
+ipython = ">=8.6.0"
 
 [tool.poetry.plugins."smqtk_plugins"]
 # DataElement
 "smqtk_dataprovider.impls.data_element.file" = "smqtk_dataprovider.impls.data_element.file"
 "smqtk_dataprovider.impls.data_element.girder" = "smqtk_dataprovider.impls.data_element.girder"
 "smqtk_dataprovider.impls.data_element.hbase" = "smqtk_dataprovider.impls.data_element.hbase"
 "smqtk_dataprovider.impls.data_element.matrix" = "smqtk_dataprovider.impls.data_element.matrix"
```

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/content_type_validator.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/content_type_validator.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/exceptions.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/exceptions.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/file.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/file.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/girder.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/girder.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/hbase.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/hbase.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/matrix.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/matrix.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/memory.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/memory.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/psql.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/psql.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_element/url.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_element/url.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_set/file.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_set/file.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_set/kvstore_backed.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_set/kvstore_backed.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_set/memory.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_set/memory.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/data_set/psql.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/data_set/psql.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/key_value_store/memory.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/key_value_store/memory.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/impls/key_value_store/postgres.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/impls/key_value_store/postgres.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/interfaces/data_element.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/interfaces/data_element.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/interfaces/data_set.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/interfaces/data_set.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/interfaces/key_value_store.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/interfaces/key_value_store.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/utils/file.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/utils/file.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/utils/postgres.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/utils/postgres.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/utils/simple_timer.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/utils/simple_timer.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/smqtk_dataprovider/utils/string.py` & `smqtk_dataprovider-0.18.0/smqtk_dataprovider/utils/string.py`

 * *Files identical despite different names*

### Comparing `smqtk_dataprovider-0.17.0/PKG-INFO` & `smqtk_dataprovider-0.18.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 Metadata-Version: 2.1
 Name: smqtk-dataprovider
-Version: 0.17.0
+Version: 0.18.0
 Summary: SMQTK Data provision abstractions and implementations
 Home-page: https://github.com/Kitware/SMQTK-Dataprovider
 License: BSD-3-Clause
 Author: Kitware, Inc.
 Author-email: smqtk-developers@kitware.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: filemagic
 Provides-Extra: girder
 Provides-Extra: psql
-Requires-Dist: file-magic (>=0.4.0,<0.5.0) ; extra == "filemagic"
-Requires-Dist: girder-client (>=3.1.3,<4.0.0) ; extra == "girder"
-Requires-Dist: numpy (>=1.21.1) ; python_version < "3.8"
-Requires-Dist: numpy (>=1.23.5) ; python_version >= "3.8"
-Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0) ; extra == "psql"
+Requires-Dist: file-magic (>=0.4.0) ; extra == "filemagic"
+Requires-Dist: girder-client (>=3.1.3) ; extra == "girder"
+Requires-Dist: numpy (>=1.23.5)
+Requires-Dist: psycopg2-binary (>=2.9.5) ; extra == "psql"
 Requires-Dist: requests (>=2.28.1)
 Requires-Dist: smqtk-core (>=0.19)
 Project-URL: Documentation, https://smqtk-dataprovider.readthedocs.io/
 Project-URL: Repository, https://github.com/Kitware/SMQTK-Dataprovider
 Description-Content-Type: text/markdown
 
 # SMQTK - Data Providers
```

