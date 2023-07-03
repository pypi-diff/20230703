# Comparing `tmp/test_measure_process_lib-1.0.8.tar.gz` & `tmp/test_measure_process_lib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_measure_process_lib-1.0.8.tar", last modified: Fri Apr 28 18:42:03 2023, max compression
+gzip compressed data, was "test_measure_process_lib-1.0.9.tar", last modified: Mon Jul  3 21:41:46 2023, max compression
```

## Comparing `test_measure_process_lib-1.0.8.tar` & `test_measure_process_lib-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    10273 2021-05-25 23:53:44.000000 test_measure_process_lib-1.0.8/LICENSE.md
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    43006 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/PKG-INFO
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    30554 2023-01-21 14:05:45.000000 test_measure_process_lib-1.0.8/README.md
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      903 2023-04-28 18:38:19.000000 test_measure_process_lib-1.0.8/pyproject.toml
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/sandbox/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      182 2023-01-21 13:48:47.000000 test_measure_process_lib-1.0.8/sandbox/set_path_for_notebooks.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       38 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/setup.cfg
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    43006 2023-04-28 18:42:03.000000 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/PKG-INFO
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      504 2023-04-28 18:42:03.000000 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)        1 2023-04-28 18:42:03.000000 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       51 2023-04-28 18:42:03.000000 test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/top_level.txt
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/tmpl/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      509 2023-04-28 18:39:01.000000 test_measure_process_lib-1.0.8/tmpl/__init__.py
-drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-04-28 18:42:03.330289 test_measure_process_lib-1.0.8/tmpl/examples/
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       60 2021-08-01 18:41:18.000000 test_measure_process_lib-1.0.8/tmpl/examples/__init__.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    12475 2023-02-25 20:07:53.000000 test_measure_process_lib-1.0.8/tmpl/examples/example_resistor_test.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     4947 2021-08-23 12:12:14.000000 test_measure_process_lib-1.0.8/tmpl/examples/resistor_example.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      182 2022-12-21 19:49:01.000000 test_measure_process_lib-1.0.8/tmpl/examples/set_path_for_notebooks.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     9822 2023-04-28 18:31:02.000000 test_measure_process_lib-1.0.8/tmpl/tmp_code_generator.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)   102795 2023-04-28 18:31:02.000000 test_measure_process_lib-1.0.8/tmpl/tmpl_core.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     4587 2021-05-25 23:41:52.000000 test_measure_process_lib-1.0.8/tmpl/tmpl_storage.py
--rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    16004 2023-02-25 20:07:53.000000 test_measure_process_lib-1.0.8/tmpl/tmpl_support.py
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-07-03 21:41:46.403487 test_measure_process_lib-1.0.9/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    10273 2021-05-25 23:53:44.000000 test_measure_process_lib-1.0.9/LICENSE.md
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    43006 2023-07-03 21:41:46.403487 test_measure_process_lib-1.0.9/PKG-INFO
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    30554 2023-01-21 14:05:45.000000 test_measure_process_lib-1.0.9/README.md
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      903 2023-07-03 21:36:46.000000 test_measure_process_lib-1.0.9/pyproject.toml
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-07-03 21:41:46.399487 test_measure_process_lib-1.0.9/sandbox/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      182 2023-01-21 13:48:47.000000 test_measure_process_lib-1.0.9/sandbox/set_path_for_notebooks.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       38 2023-07-03 21:41:46.403487 test_measure_process_lib-1.0.9/setup.cfg
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-07-03 21:41:46.403487 test_measure_process_lib-1.0.9/test_measure_process_lib.egg-info/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    43006 2023-07-03 21:41:46.000000 test_measure_process_lib-1.0.9/test_measure_process_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      504 2023-07-03 21:41:46.000000 test_measure_process_lib-1.0.9/test_measure_process_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)        1 2023-07-03 21:41:46.000000 test_measure_process_lib-1.0.9/test_measure_process_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       51 2023-07-03 21:41:46.000000 test_measure_process_lib-1.0.9/test_measure_process_lib.egg-info/top_level.txt
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-07-03 21:41:46.403487 test_measure_process_lib-1.0.9/tmpl/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      509 2023-07-03 21:37:12.000000 test_measure_process_lib-1.0.9/tmpl/__init__.py
+drwxrwxr-x   0 redlegjed  (1001) redlegjed  (1001)        0 2023-07-03 21:41:46.403487 test_measure_process_lib-1.0.9/tmpl/examples/
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)       60 2021-08-01 18:41:18.000000 test_measure_process_lib-1.0.9/tmpl/examples/__init__.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    12475 2023-02-25 20:07:53.000000 test_measure_process_lib-1.0.9/tmpl/examples/example_resistor_test.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     4947 2021-08-23 12:12:14.000000 test_measure_process_lib-1.0.9/tmpl/examples/resistor_example.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)      182 2022-12-21 19:49:01.000000 test_measure_process_lib-1.0.9/tmpl/examples/set_path_for_notebooks.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     9822 2023-04-28 18:31:02.000000 test_measure_process_lib-1.0.9/tmpl/tmp_code_generator.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)   103275 2023-07-03 21:36:03.000000 test_measure_process_lib-1.0.9/tmpl/tmpl_core.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)     4587 2021-05-25 23:41:52.000000 test_measure_process_lib-1.0.9/tmpl/tmpl_storage.py
+-rw-rw-r--   0 redlegjed  (1001) redlegjed  (1001)    16004 2023-02-25 20:07:53.000000 test_measure_process_lib-1.0.9/tmpl/tmpl_support.py
```

### Comparing `test_measure_process_lib-1.0.8/LICENSE.md` & `test_measure_process_lib-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.8/PKG-INFO` & `test_measure_process_lib-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_measure_process_lib
-Version: 1.0.8
+Version: 1.0.9
 Summary: Test, Measure and Process library. Framework for lab experiments.
 Author-email: RedLegJed <rlj_pypi@nym.hush.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `test_measure_process_lib-1.0.8/README.md` & `test_measure_process_lib-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.8/pyproject.toml` & `test_measure_process_lib-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "test_measure_process_lib"
-version = "1.0.8"
+version = "1.0.9"
 description = "Test, Measure and Process library. Framework for lab experiments."
 readme = "README.md"
 authors = [{ name = "RedLegJed", email = "rlj_pypi@nym.hush.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `test_measure_process_lib-1.0.8/test_measure_process_lib.egg-info/PKG-INFO` & `test_measure_process_lib-1.0.9/test_measure_process_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-measure-process-lib
-Version: 1.0.8
+Version: 1.0.9
 Summary: Test, Measure and Process library. Framework for lab experiments.
 Author-email: RedLegJed <rlj_pypi@nym.hush.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `test_measure_process_lib-1.0.8/tmpl/examples/example_resistor_test.py` & `test_measure_process_lib-1.0.9/tmpl/examples/example_resistor_test.py`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.8/tmpl/examples/resistor_example.py` & `test_measure_process_lib-1.0.9/tmpl/examples/resistor_example.py`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.8/tmpl/tmp_code_generator.py` & `test_measure_process_lib-1.0.9/tmpl/tmp_code_generator.py`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.8/tmpl/tmpl_core.py` & `test_measure_process_lib-1.0.9/tmpl/tmpl_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2029,26 +2029,35 @@
 
         Parameters
         ----------
         object : Measurement or SetupConditions class
             A TMPL object e.g. any class based on AbstractMeasurement or
             AbstractSetupConditions
         """
-        methods = inspect.getmembers(object, predicate=inspect.ismethod)
-        methods = [m[0] for m in methods if not m[0].startswith('_')]
+        # Get list of all attributes of the object
+        methods = dir(object)
+        # Filter out private methods
+        methods = [m for m in methods if not m.startswith('_')]
 
-        # for attr in [a for a in dir(object) if not a.startswith('_')]:
+        # Check attributes to see if they have an 'is_service' property
+        # if they do then add them to self.services ObjDict
         for attr in methods:
-            attr_obj = getattr(object,attr)
+            # Use the inspect module getattr_static because it does not
+            # execute code in the attribute
+            attr_obj = inspect.getattr_static(object,attr)
 
             try:
 
                 if hasattr(attr_obj,'is_service'):
                     # print(f'{attr_obj.__name__} : is a service')
-                    self.services[attr_obj.__name__] = attr_obj
+                    # Add reference to service method
+                    # - this needs to be the proper attribute obtained from
+                    #   getattr(), the inspect.getattr_static doesn't work
+                    #   for this 
+                    self.services[attr_obj.__name__] = getattr(object,attr)
 
             except:
                 # Ignore failures, which are usually the ObjDict properties
                 # print(f'Weird object [{attr}]')
                 pass
```

### Comparing `test_measure_process_lib-1.0.8/tmpl/tmpl_storage.py` & `test_measure_process_lib-1.0.9/tmpl/tmpl_storage.py`

 * *Files identical despite different names*

### Comparing `test_measure_process_lib-1.0.8/tmpl/tmpl_support.py` & `test_measure_process_lib-1.0.9/tmpl/tmpl_support.py`

 * *Files identical despite different names*

