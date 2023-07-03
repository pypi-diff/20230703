# Comparing `tmp/phanos-0.0.2.tar.gz` & `tmp/phanos-0.0.3.tar.gz`

## Comparing `phanos-0.0.2.tar` & `phanos-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.2/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.2/Pipfile.lock
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 phanos-0.0.2/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 phanos-0.0.2/src/phanos/__init__.py
--rw-r--r--   0        0        0    14820 2020-02-02 00:00:00.000000 phanos-0.0.2/src/phanos/metrics.py
--rw-r--r--   0        0        0    15292 2020-02-02 00:00:00.000000 phanos-0.0.2/src/phanos/publisher.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 phanos-0.0.2/src/phanos/tree.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 phanos-0.0.2/test/__init__.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 phanos-0.0.2/test/dummy_api.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 phanos-0.0.2/test/requirements.txt
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.2/test/run_tests.py
--rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 phanos-0.0.2/test/test_metric.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.2/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.2/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.2/LICENSE
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 phanos-0.0.2/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 phanos-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 phanos-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.3/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.3/Pipfile.lock
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 phanos-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.3/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 phanos-0.0.3/src/phanos/__init__.py
+-rw-r--r--   0        0        0    14820 2020-02-02 00:00:00.000000 phanos-0.0.3/src/phanos/metrics.py
+-rw-r--r--   0        0        0    15292 2020-02-02 00:00:00.000000 phanos-0.0.3/src/phanos/publisher.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 phanos-0.0.3/src/phanos/tree.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 phanos-0.0.3/test/__init__.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 phanos-0.0.3/test/dummy_api.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 phanos-0.0.3/test/requirements.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.3/test/run_tests.py
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 phanos-0.0.3/test/test_metric.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.3/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 phanos-0.0.3/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 phanos-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 phanos-0.0.3/PKG-INFO
```

### Comparing `phanos-0.0.2/Pipfile.lock` & `phanos-0.0.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/deactivate/bin/Activate.ps1` & `phanos-0.0.3/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/deactivate/bin/activate` & `phanos-0.0.3/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/deactivate/bin/activate.csh` & `phanos-0.0.3/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/deactivate/bin/activate.fish` & `phanos-0.0.3/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/src/phanos/metrics.py` & `phanos-0.0.3/src/phanos/metrics.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/src/phanos/publisher.py` & `phanos-0.0.3/src/phanos/publisher.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/src/phanos/tree.py` & `phanos-0.0.3/src/phanos/tree.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/test/dummy_api.py` & `phanos-0.0.3/test/dummy_api.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/test/run_tests.py` & `phanos-0.0.3/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/test/test_metric.py` & `phanos-0.0.3/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/test/testing_data.py` & `phanos-0.0.3/test/testing_data.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/.gitignore` & `phanos-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/LICENSE` & `phanos-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/README.md` & `phanos-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `phanos-0.0.2/pyproject.toml` & `phanos-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
+dependencies = [
+    "Flask>=2.2.3",
+    "imp_prof>=0.1.0",
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-
 [project.urls]
 "Homepage" = "https://github.com/kajotgames/phanos"
-"Bug Tracker" = "https://github.com/kajotgames/phanos/issues"
+"Bug Tracker" = "https://github.com/kajotgames/phanos/issues"
+
+[coverage.run]
+branch = true
+source = [
+    "src/phanos",
+    "test",
+]
+
+[coverage.paths]
+source = "phanos"
```

### Comparing `phanos-0.0.2/PKG-INFO` & `phanos-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.6
+Requires-Dist: flask>=2.2.3
+Requires-Dist: imp-prof>=0.1.0
 Description-Content-Type: text/markdown
 
 # PHANOS
 Python client to gather data for Prometheus logging in server with multiple instances and workers.
 
 ## Profiling
```

