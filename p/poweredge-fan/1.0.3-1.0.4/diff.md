# Comparing `tmp/poweredge_fan-1.0.3.tar.gz` & `tmp/poweredge_fan-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poweredge_fan-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "poweredge_fan-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `poweredge_fan-1.0.3.tar` & `poweredge_fan-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      521 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      701 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0     5338 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/.gitignore
--rw-r--r--   0        0        0     4435 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/README.md
--rw-r--r--   0        0        0      298 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/poweredge_fan.service
--rw-r--r--   0        0        0        0 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/poweredge_fan/__init__.py
--rw-r--r--   0        0        0       71 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/poweredge_fan/hardware/__init__.py
--rw-r--r--   0        0        0     2110 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/poweredge_fan/hardware/poweredge.py
--rw-r--r--   0        0        0      579 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/poweredge_fan/hardware/sensors.py
--rw-r--r--   0        0        0     3646 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/poweredge_fan/poweredge_fan.py
--rw-r--r--   0        0        0      558 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       10 2023-07-03 07:37:59.929516 poweredge_fan-1.0.3/requirements.txt
--rw-r--r--   0        0        0     4861 1970-01-01 00:00:00.000000 poweredge_fan-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      521 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      701 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     5338 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/.gitignore
+-rw-r--r--   0        0        0     4435 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/README.md
+-rw-r--r--   0        0        0      298 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/poweredge_fan.service
+-rw-r--r--   0        0        0        0 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/poweredge_fan/__init__.py
+-rw-r--r--   0        0        0       71 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/poweredge_fan/hardware/__init__.py
+-rw-r--r--   0        0        0     2110 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/poweredge_fan/hardware/poweredge.py
+-rw-r--r--   0        0        0      579 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/poweredge_fan/hardware/sensors.py
+-rw-r--r--   0        0        0     3662 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/poweredge_fan/poweredge_fan.py
+-rw-r--r--   0        0        0      558 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       10 2023-07-03 07:42:42.662765 poweredge_fan-1.0.4/requirements.txt
+-rw-r--r--   0        0        0     4861 1970-01-01 00:00:00.000000 poweredge_fan-1.0.4/PKG-INFO
```

### Comparing `poweredge_fan-1.0.3/.github/workflows/build.yml` & `poweredge_fan-1.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `poweredge_fan-1.0.3/.github/workflows/publish.yml` & `poweredge_fan-1.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `poweredge_fan-1.0.3/.gitignore` & `poweredge_fan-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `poweredge_fan-1.0.3/README.md` & `poweredge_fan-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `poweredge_fan-1.0.3/poweredge_fan/hardware/poweredge.py` & `poweredge_fan-1.0.4/poweredge_fan/hardware/poweredge.py`

 * *Files identical despite different names*

### Comparing `poweredge_fan-1.0.3/poweredge_fan/hardware/sensors.py` & `poweredge_fan-1.0.4/poweredge_fan/hardware/sensors.py`

 * *Files identical despite different names*

### Comparing `poweredge_fan-1.0.3/poweredge_fan/poweredge_fan.py` & `poweredge_fan-1.0.4/poweredge_fan/poweredge_fan.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         except TimeoutExpired as e:
             print("Timeout expired, skipping update")
             print(e)
             ipmi.set_fan_automatic()
             time.sleep(1)
 
 def main():
+    global ipmi
     args = arg_parser.parse_args()
     ipmi = IPMIControl(args.host, args.username, args.password)
     try:
         loop()
     finally:
         ipmi.set_fan_automatic()
```

### Comparing `poweredge_fan-1.0.3/pyproject.toml` & `poweredge_fan-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "poweredge_fan"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     {name = "Jackie Yang", email = "jackie@jackieyang.me"},
 ]
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License", "Programming Language :: Python :: 3"]
 urls = {Source = "https://github.com/valkjsaaa/PyPowerEdgeFan"}
 dependencies = [
```

### Comparing `poweredge_fan-1.0.3/PKG-INFO` & `poweredge_fan-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poweredge_fan
-Version: 1.0.3
+Version: 1.0.4
 Summary: PyPowerEdgeFan is a Python-based PID fan controller for Dell PowerEdge servers.
 Author-email: Jackie Yang <jackie@jackieyang.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: PySensors
 Project-URL: Source, https://github.com/valkjsaaa/PyPowerEdgeFan
```

