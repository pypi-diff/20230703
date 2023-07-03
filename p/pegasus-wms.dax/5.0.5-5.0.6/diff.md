# Comparing `tmp/pegasus-wms.dax-5.0.5.tar.gz` & `tmp/pegasus-wms.dax-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../../dist/pegasus-wms.dax-5.0.5.tar", last modified: Fri Feb 17 18:24:04 2023, max compression
+gzip compressed data, was "pegasus-wms.dax-5.0.6.tar", last modified: Mon Jul  3 15:44:37 2023, max compression
```

## Comparing `pegasus-wms.dax-5.0.5.tar` & `pegasus-wms.dax-5.0.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/src/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/src/Pegasus/
--rw-r--r--   0 bamboo     (550) users      (100)    74106 2023-02-17 18:23:44.000000 pegasus-wms.dax-5.0.5/src/Pegasus/DAX3.py
--rw-r--r--   0 bamboo     (550) users      (100)       65 2023-02-17 18:23:44.000000 pegasus-wms.dax-5.0.5/src/Pegasus/__init__.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/src/pegasus_wms.dax.egg-info/
--rw-r--r--   0 bamboo     (550) users      (100)     1757 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/src/pegasus_wms.dax.egg-info/PKG-INFO
--rw-r--r--   0 bamboo     (550) users      (100)      348 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/src/pegasus_wms.dax.egg-info/SOURCES.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/src/pegasus_wms.dax.egg-info/dependency_links.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/src/pegasus_wms.dax.egg-info/not-zip-safe
--rw-r--r--   0 bamboo     (550) users      (100)       11 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/src/pegasus_wms.dax.egg-info/requires.txt
--rw-r--r--   0 bamboo     (550) users      (100)        8 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/src/pegasus_wms.dax.egg-info/top_level.txt
--rw-r--r--   0 bamboo     (550) users      (100)    11368 2023-02-17 18:23:44.000000 pegasus-wms.dax-5.0.5/LICENSE
--rw-r--r--   0 bamboo     (550) users      (100)       60 2023-02-17 18:23:44.000000 pegasus-wms.dax-5.0.5/MANIFEST.in
--rw-r--r--   0 bamboo     (550) users      (100)      204 2023-02-17 18:23:44.000000 pegasus-wms.dax-5.0.5/README.md
--rw-r--r--   0 bamboo     (550) users      (100)      176 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/setup.cfg
--rw-r--r--   0 bamboo     (550) users      (100)     2393 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/setup.py
--rw-r--r--   0 bamboo     (550) users      (100)     1757 2023-02-17 18:24:04.000000 pegasus-wms.dax-5.0.5/PKG-INFO
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:37.419379 pegasus-wms.dax-5.0.6/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    11368 2023-07-03 15:42:39.000000 pegasus-wms.dax-5.0.6/LICENSE
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       60 2023-07-03 15:42:39.000000 pegasus-wms.dax-5.0.6/MANIFEST.in
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1716 2023-07-03 15:44:37.419379 pegasus-wms.dax-5.0.6/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      204 2023-07-03 15:42:39.000000 pegasus-wms.dax-5.0.6/README.md
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      601 2023-07-03 15:42:39.000000 pegasus-wms.dax-5.0.6/pyproject.toml
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      176 2023-07-03 15:44:37.419379 pegasus-wms.dax-5.0.6/setup.cfg
+-rw-------   0 rynge     (1000) rynge     (1000)     2393 2023-07-03 15:44:36.000000 pegasus-wms.dax-5.0.6/setup.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:37.415379 pegasus-wms.dax-5.0.6/src/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:37.415379 pegasus-wms.dax-5.0.6/src/Pegasus/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    74106 2023-07-03 15:42:39.000000 pegasus-wms.dax-5.0.6/src/Pegasus/DAX3.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       65 2023-07-03 15:42:39.000000 pegasus-wms.dax-5.0.6/src/Pegasus/__init__.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:37.419379 pegasus-wms.dax-5.0.6/src/pegasus_wms.dax.egg-info/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1716 2023-07-03 15:44:36.000000 pegasus-wms.dax-5.0.6/src/pegasus_wms.dax.egg-info/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      371 2023-07-03 15:44:37.000000 pegasus-wms.dax-5.0.6/src/pegasus_wms.dax.egg-info/SOURCES.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:36.000000 pegasus-wms.dax-5.0.6/src/pegasus_wms.dax.egg-info/dependency_links.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:36.000000 pegasus-wms.dax-5.0.6/src/pegasus_wms.dax.egg-info/not-zip-safe
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       11 2023-07-03 15:44:36.000000 pegasus-wms.dax-5.0.6/src/pegasus_wms.dax.egg-info/requires.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        8 2023-07-03 15:44:36.000000 pegasus-wms.dax-5.0.6/src/pegasus_wms.dax.egg-info/top_level.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1570 2023-07-03 15:42:39.000000 pegasus-wms.dax-5.0.6/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pegasus-wms.dax-5.0.5/src/Pegasus/DAX3.py` & `pegasus-wms.dax-5.0.6/src/Pegasus/DAX3.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.dax-5.0.5/src/pegasus_wms.dax.egg-info/PKG-INFO` & `pegasus-wms.dax-5.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms.dax
-Version: 5.0.5
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Python API
 Home-page: http://pegasus.isi.edu
 Author: Pegasus Team
 Author-email: pegasus@isi.edu
 License: Apache2
 Project-URL: Documentation, https://pegasus.isi.edu/documentation/
 Project-URL: Changes, https://pegasus.isi.edu/blog/?category_name=Release
 Project-URL: Source Code, https://github.com/pegasus-isi/pegasus
 Project-URL: Issue Tracker, https://jira.isi.edu/projects/PM/issues
-Description: Pegasus Workflow Management Python DAX API
-        ==========================================
-        
-        The `Pegasus.DAX3` API has been deprecated and will be removed in v5.1.0. Please use the new API released in v5.0.0.
-        
 Keywords: scientific workflows
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
@@ -33,7 +27,13 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=2.6,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Pegasus Workflow Management Python DAX API
+==========================================
+
+The `Pegasus.DAX3` API has been deprecated and will be removed in v5.1.0. Please use the new API released in v5.0.0.
```

### Comparing `pegasus-wms.dax-5.0.5/LICENSE` & `pegasus-wms.dax-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasus-wms.dax-5.0.5/setup.py` & `pegasus-wms.dax-5.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #
 def read(fname):
     return open(os.path.join(src_dir, fname)).read()
 
 
 setup(
     name="pegasus-wms.dax",
-    version="5.0.5",
+    version="5.0.6",
     author="Pegasus Team",
     author_email="pegasus@isi.edu",
     description="Pegasus Workflow Management System Python API",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     license="Apache2",
     url="http://pegasus.isi.edu",
```

### Comparing `pegasus-wms.dax-5.0.5/PKG-INFO` & `pegasus-wms.dax-5.0.6/src/pegasus_wms.dax.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms.dax
-Version: 5.0.5
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Python API
 Home-page: http://pegasus.isi.edu
 Author: Pegasus Team
 Author-email: pegasus@isi.edu
 License: Apache2
 Project-URL: Documentation, https://pegasus.isi.edu/documentation/
 Project-URL: Changes, https://pegasus.isi.edu/blog/?category_name=Release
 Project-URL: Source Code, https://github.com/pegasus-isi/pegasus
 Project-URL: Issue Tracker, https://jira.isi.edu/projects/PM/issues
-Description: Pegasus Workflow Management Python DAX API
-        ==========================================
-        
-        The `Pegasus.DAX3` API has been deprecated and will be removed in v5.1.0. Please use the new API released in v5.0.0.
-        
 Keywords: scientific workflows
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
@@ -33,7 +27,13 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=2.6,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Pegasus Workflow Management Python DAX API
+==========================================
+
+The `Pegasus.DAX3` API has been deprecated and will be removed in v5.1.0. Please use the new API released in v5.0.0.
```

