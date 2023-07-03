# Comparing `tmp/pegasus-wms.common-5.0.5.tar.gz` & `tmp/pegasus-wms.common-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../../dist/pegasus-wms.common-5.0.5.tar", last modified: Fri Feb 17 18:24:04 2023, max compression
+gzip compressed data, was "pegasus-wms.common-5.0.6.tar", last modified: Mon Jul  3 15:44:34 2023, max compression
```

## Comparing `pegasus-wms.common-5.0.5.tar` & `pegasus-wms.common-5.0.6.tar`

### file list

```diff
@@ -1,34 +1,43 @@
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/Pegasus/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/Pegasus/client/
--rw-r--r--   0 bamboo     (550) users      (100)        0 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/client/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)    26875 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/client/_client.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/
--rw-r--r--   0 bamboo     (550) users      (100)     1282 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)     7050 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/_compat.py
--rw-r--r--   0 bamboo     (550) users      (100)      447 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/_config.py
--rw-r--r--   0 bamboo     (550) users      (100)     9414 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/_funcs.py
--rw-r--r--   0 bamboo     (550) users      (100)    69470 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/_make.py
--rw-r--r--   0 bamboo     (550) users      (100)     2066 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/_version_info.py
--rw-r--r--   0 bamboo     (550) users      (100)     2024 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/converters.py
--rw-r--r--   0 bamboo     (550) users      (100)     1568 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/exceptions.py
--rw-r--r--   0 bamboo     (550) users      (100)     1033 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/filters.py
--rw-r--r--   0 bamboo     (550) users      (100)    10988 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/validators.py
--rw-r--r--   0 bamboo     (550) users      (100)     5872 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/braindump.py
--rw-r--r--   0 bamboo     (550) users      (100)     2623 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/json.py
--rw-r--r--   0 bamboo     (550) users      (100)     2912 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/src/Pegasus/yaml.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/pegasus_wms.common.egg-info/
--rw-r--r--   0 bamboo     (550) users      (100)     1933 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/pegasus_wms.common.egg-info/PKG-INFO
--rw-r--r--   0 bamboo     (550) users      (100)      811 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/pegasus_wms.common.egg-info/SOURCES.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/pegasus_wms.common.egg-info/dependency_links.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/pegasus_wms.common.egg-info/not-zip-safe
--rw-r--r--   0 bamboo     (550) users      (100)       11 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/pegasus_wms.common.egg-info/requires.txt
--rw-r--r--   0 bamboo     (550) users      (100)        8 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/src/pegasus_wms.common.egg-info/top_level.txt
--rw-r--r--   0 bamboo     (550) users      (100)    11368 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/LICENSE
--rw-r--r--   0 bamboo     (550) users      (100)       60 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/MANIFEST.in
--rw-r--r--   0 bamboo     (550) users      (100)      425 2023-02-17 18:23:44.000000 pegasus-wms.common-5.0.5/README.md
--rw-r--r--   0 bamboo     (550) users      (100)      176 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/setup.cfg
--rw-r--r--   0 bamboo     (550) users      (100)     2700 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/setup.py
--rw-r--r--   0 bamboo     (550) users      (100)     1933 2023-02-17 18:24:04.000000 pegasus-wms.common-5.0.5/PKG-INFO
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:34.699348 pegasus-wms.common-5.0.6/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    11368 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/LICENSE
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       60 2023-07-03 15:42:39.000000 pegasus-wms.common-5.0.6/MANIFEST.in
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1812 2023-07-03 15:44:34.699348 pegasus-wms.common-5.0.6/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      425 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/README.md
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      615 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/pyproject.toml
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      176 2023-07-03 15:44:34.699348 pegasus-wms.common-5.0.6/setup.cfg
+-rw-------   0 rynge     (1000) rynge     (1000)     2700 2023-07-03 15:44:33.000000 pegasus-wms.common-5.0.6/setup.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:34.691348 pegasus-wms.common-5.0.6/src/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:34.691348 pegasus-wms.common-5.0.6/src/Pegasus/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     5872 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/braindump.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:34.691348 pegasus-wms.common-5.0.6/src/Pegasus/client/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        0 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/client/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    26874 2023-07-03 15:42:39.000000 pegasus-wms.common-5.0.6/src/Pegasus/client/_client.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2623 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/json.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:34.691348 pegasus-wms.common-5.0.6/src/Pegasus/vendor/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:34.695348 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1282 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     8252 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/__init__.pyi
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     7050 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_compat.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      447 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_config.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     9414 2023-07-03 15:42:39.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_funcs.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    69470 2023-07-03 15:42:39.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_make.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2066 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_version_info.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      209 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_version_info.pyi
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2024 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/converters.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      346 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/converters.pyi
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1568 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/exceptions.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      458 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/exceptions.pyi
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1033 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/filters.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      215 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/filters.pyi
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        0 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/py.typed
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    10988 2023-07-03 15:42:39.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/validators.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1855 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/validators.pyi
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2912 2023-06-30 20:04:01.000000 pegasus-wms.common-5.0.6/src/Pegasus/yaml.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:34.699348 pegasus-wms.common-5.0.6/src/pegasus_wms.common.egg-info/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1812 2023-07-03 15:44:33.000000 pegasus-wms.common-5.0.6/src/pegasus_wms.common.egg-info/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1099 2023-07-03 15:44:34.000000 pegasus-wms.common-5.0.6/src/pegasus_wms.common.egg-info/SOURCES.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:33.000000 pegasus-wms.common-5.0.6/src/pegasus_wms.common.egg-info/dependency_links.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:33.000000 pegasus-wms.common-5.0.6/src/pegasus_wms.common.egg-info/not-zip-safe
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       11 2023-07-03 15:44:33.000000 pegasus-wms.common-5.0.6/src/pegasus_wms.common.egg-info/requires.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        8 2023-07-03 15:44:33.000000 pegasus-wms.common-5.0.6/src/pegasus_wms.common.egg-info/top_level.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1768 2023-07-03 15:42:39.000000 pegasus-wms.common-5.0.6/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/client/_client.py` & `pegasus-wms.common-5.0.6/src/Pegasus/client/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 
         # always use --json option
         cmd.append("--json")
 
         self._log.info("\n################\n# pegasus-plan #\n################")
 
         # don't stream stdout from planner, as this will be json output
-        rv = self._exec(cmd, stream_stdout=False, stream_stderr=True)
+        rv = self._exec(cmd, stream_stdout=True, stream_stderr=True)
 
         json_output = rv.json
         submit_dir = json_output["submit_dir"]
 
         # Some tools (launch-bamboo-script, ensemble-mananager) parse submit directory from
         # planner output. Therefore we need to log the following and retain the structure
         # of planner output.
```

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/__init__.py` & `pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/_compat.py` & `pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_compat.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/_funcs.py` & `pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_funcs.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/_make.py` & `pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_make.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/_version_info.py` & `pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/_version_info.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/converters.py` & `pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/converters.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/exceptions.py` & `pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/exceptions.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/filters.py` & `pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/filters.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/vendor/attr/validators.py` & `pegasus-wms.common-5.0.6/src/Pegasus/vendor/attr/validators.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/braindump.py` & `pegasus-wms.common-5.0.6/src/Pegasus/braindump.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/json.py` & `pegasus-wms.common-5.0.6/src/Pegasus/json.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/Pegasus/yaml.py` & `pegasus-wms.common-5.0.6/src/Pegasus/yaml.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/src/pegasus_wms.common.egg-info/PKG-INFO` & `pegasus-wms.common-5.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms.common
-Version: 5.0.5
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Python Commons
 Home-page: http://pegasus.isi.edu
 Author: Pegasus Team
 Author-email: pegasus@isi.edu
 License: Apache2
 Project-URL: Documentation, https://pegasus.isi.edu/documentation/
 Project-URL: Changes, https://pegasus.isi.edu/blog/?category_name=Release
 Project-URL: Source Code, https://github.com/pegasus-isi/pegasus
 Project-URL: Issue Tracker, https://jira.isi.edu/projects/PM/issues
-Description: Pegasus Workflow Management System Python API
-        =============================================
-        
-        This package contains the Python APIs for Pegasus WMS, including:
-        
-        1. The DAX API (Versions 2 and 3)
-        2. The PDAX API (Version 2)
-        3. The monitoring API
-        4. The Stampede database API
-        5. The Pegasus statistics API
-        6. The Pegasus plots API
-        7. Misc. Pegasus utilities
-        8. The pegasus service, including the ensemble manager and dashboard
-        
-        
 Keywords: scientific workflows
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,7 +25,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Pegasus Workflow Management System Python API
+=============================================
+
+This package contains the Python APIs for Pegasus WMS, including:
+
+1. The DAX API (Versions 2 and 3)
+2. The PDAX API (Version 2)
+3. The monitoring API
+4. The Stampede database API
+5. The Pegasus statistics API
+6. The Pegasus plots API
+7. Misc. Pegasus utilities
+8. The pegasus service, including the ensemble manager and dashboard
+
```

### Comparing `pegasus-wms.common-5.0.5/src/pegasus_wms.common.egg-info/SOURCES.txt` & `pegasus-wms.common-5.0.6/src/pegasus_wms.common.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
+tox.ini
 src/Pegasus/braindump.py
 src/Pegasus/json.py
 src/Pegasus/yaml.py
 src/Pegasus/client/__init__.py
 src/Pegasus/client/_client.py
 src/Pegasus/vendor/attr/__init__.py
+src/Pegasus/vendor/attr/__init__.pyi
 src/Pegasus/vendor/attr/_compat.py
 src/Pegasus/vendor/attr/_config.py
 src/Pegasus/vendor/attr/_funcs.py
 src/Pegasus/vendor/attr/_make.py
 src/Pegasus/vendor/attr/_version_info.py
+src/Pegasus/vendor/attr/_version_info.pyi
 src/Pegasus/vendor/attr/converters.py
+src/Pegasus/vendor/attr/converters.pyi
 src/Pegasus/vendor/attr/exceptions.py
+src/Pegasus/vendor/attr/exceptions.pyi
 src/Pegasus/vendor/attr/filters.py
+src/Pegasus/vendor/attr/filters.pyi
+src/Pegasus/vendor/attr/py.typed
 src/Pegasus/vendor/attr/validators.py
+src/Pegasus/vendor/attr/validators.pyi
 src/pegasus_wms.common.egg-info/PKG-INFO
 src/pegasus_wms.common.egg-info/SOURCES.txt
 src/pegasus_wms.common.egg-info/dependency_links.txt
 src/pegasus_wms.common.egg-info/not-zip-safe
 src/pegasus_wms.common.egg-info/requires.txt
 src/pegasus_wms.common.egg-info/top_level.txt
```

### Comparing `pegasus-wms.common-5.0.5/LICENSE` & `pegasus-wms.common-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasus-wms.common-5.0.5/setup.py` & `pegasus-wms.common-5.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             pkgs.append(os.path.join(root, pkg).replace("/", "."))
 
     return pkgs
 
 
 setup(
     name="pegasus-wms.common",
-    version="5.0.5",
+    version="5.0.6",
     author="Pegasus Team",
     author_email="pegasus@isi.edu",
     description="Pegasus Workflow Management System Python Commons",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     license="Apache2",
     url="http://pegasus.isi.edu",
```

### Comparing `pegasus-wms.common-5.0.5/PKG-INFO` & `pegasus-wms.common-5.0.6/src/pegasus_wms.common.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms.common
-Version: 5.0.5
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Python Commons
 Home-page: http://pegasus.isi.edu
 Author: Pegasus Team
 Author-email: pegasus@isi.edu
 License: Apache2
 Project-URL: Documentation, https://pegasus.isi.edu/documentation/
 Project-URL: Changes, https://pegasus.isi.edu/blog/?category_name=Release
 Project-URL: Source Code, https://github.com/pegasus-isi/pegasus
 Project-URL: Issue Tracker, https://jira.isi.edu/projects/PM/issues
-Description: Pegasus Workflow Management System Python API
-        =============================================
-        
-        This package contains the Python APIs for Pegasus WMS, including:
-        
-        1. The DAX API (Versions 2 and 3)
-        2. The PDAX API (Version 2)
-        3. The monitoring API
-        4. The Stampede database API
-        5. The Pegasus statistics API
-        6. The Pegasus plots API
-        7. Misc. Pegasus utilities
-        8. The pegasus service, including the ensemble manager and dashboard
-        
-        
 Keywords: scientific workflows
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,7 +25,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Pegasus Workflow Management System Python API
+=============================================
+
+This package contains the Python APIs for Pegasus WMS, including:
+
+1. The DAX API (Versions 2 and 3)
+2. The PDAX API (Version 2)
+3. The monitoring API
+4. The Stampede database API
+5. The Pegasus statistics API
+6. The Pegasus plots API
+7. Misc. Pegasus utilities
+8. The pegasus service, including the ensemble manager and dashboard
+
```

