# Comparing `tmp/phanos-0.0.1.tar.gz` & `tmp/phanos-0.0.2.tar.gz`

## Comparing `phanos-0.0.1.tar` & `phanos-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,31 @@
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 phanos-0.0.1/Pipfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.1/requierements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.1/src/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 phanos-0.0.1/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.1/LICENSE
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 phanos-0.0.1/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 phanos-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 phanos-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.2/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.2/Pipfile.lock
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 phanos-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.2/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 phanos-0.0.2/src/phanos/__init__.py
+-rw-r--r--   0        0        0    14820 2020-02-02 00:00:00.000000 phanos-0.0.2/src/phanos/metrics.py
+-rw-r--r--   0        0        0    15292 2020-02-02 00:00:00.000000 phanos-0.0.2/src/phanos/publisher.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 phanos-0.0.2/src/phanos/tree.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 phanos-0.0.2/test/__init__.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 phanos-0.0.2/test/dummy_api.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 phanos-0.0.2/test/requirements.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.2/test/run_tests.py
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 phanos-0.0.2/test/test_metric.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.2/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 phanos-0.0.2/README.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 phanos-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 phanos-0.0.2/PKG-INFO
```

### Comparing `phanos-0.0.1/LICENSE` & `phanos-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.0.1/pyproject.toml` & `phanos-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
 classifiers = [
```

