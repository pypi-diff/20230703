# Comparing `tmp/rfcontrolpy-0.0.4.tar.gz` & `tmp/rfcontrolpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcontrolpy-0.0.4.tar", last modified: Mon May 15 22:20:57 2023, max compression
+gzip compressed data, was "rfcontrolpy-0.0.5.tar", last modified: Mon Jul  3 21:16:30 2023, max compression
```

## Comparing `rfcontrolpy-0.0.4.tar` & `rfcontrolpy-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.043381 rfcontrolpy-0.0.4/rfcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/rfcontrol/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/dimmer1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/dimmer2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/generic2.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/pir3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch11.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch25.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch7.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/weather19.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/weather7.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-15 22:20:57.000000 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-15 22:20:57.000000 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:20:57.000000 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 22:20:57.000000 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    97702 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:16:30.809610 rfcontrolpy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-03 21:16:30.809610 rfcontrolpy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:16:30.805610 rfcontrolpy-0.0.5/rfcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:16:30.805610 rfcontrolpy-0.0.5/rfcontrol/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/dimmer1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/dimmer2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/generic2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/pir1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/pir2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/pir3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/pir6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/switch8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/weather19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/protocols/weather7.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/rfcontrol/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:16:30.809610 rfcontrolpy-0.0.5/rfcontrolpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-03 21:16:30.000000 rfcontrolpy-0.0.5/rfcontrolpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 21:16:30.000000 rfcontrolpy-0.0.5/rfcontrolpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:16:30.000000 rfcontrolpy-0.0.5/rfcontrolpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 21:16:30.000000 rfcontrolpy-0.0.5/rfcontrolpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 21:16:30.809610 rfcontrolpy-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:16:30.809610 rfcontrolpy-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    97702 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 21:16:21.000000 rfcontrolpy-0.0.5/tests/test_helpers.py
```

### Comparing `rfcontrolpy-0.0.4/LICENSE` & `rfcontrolpy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/PKG-INFO` & `rfcontrolpy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfcontrolpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library with protocol support for different 433MHz switches and weather stations for the RFControl Arduino library.
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/rfcontrolpy
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/rfcontrolpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `rfcontrolpy-0.0.4/README.md` & `rfcontrolpy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/pyproject.toml` & `rfcontrolpy-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rfcontrolpy"
-version = "0.0.4"
+version = "0.0.5"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Library with protocol support for different 433MHz switches and weather stations for the RFControl Arduino library."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `rfcontrolpy-0.0.4/rfcontrol/controller.py` & `rfcontrolpy-0.0.5/rfcontrol/controller.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/helpers.py` & `rfcontrolpy-0.0.5/rfcontrol/helpers.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/__init__.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/_skeleton.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/_skeleton.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/dimmer1.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/dimmer1.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/dimmer2.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/dimmer2.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/generic.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/generic.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/generic2.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/generic2.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/pir3.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/pir3.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     # 011010011010010110101010010101101010011001100110100101100101101002
 
     # We first map the sequences to binary.
     binary = pulses2binary(pulses, pulses2binary_mapping)
     # Binary is now something like:
     # 10010011000011100010101001101100
 
+    if binary is None:
+        return None
+
     # Now we extract the data from that string.
     decoded = {
         "id": int(binary[0:16], 2),
         "unit": int(binary[16:32], 2),
         "state": True,
     }
     logger.debug(decoded)
```

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch1.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch1.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch10.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch10.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch11.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch11.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch2.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch2.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch25.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch25.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch3.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch3.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch4.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch4.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch5.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch5.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch6.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch6.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch7.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch7.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/switch8.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/switch8.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/weather19.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/weather19.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrol/protocols/weather7.py` & `rfcontrolpy-0.0.5/rfcontrol/protocols/weather7.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/rfcontrolpy.egg-info/PKG-INFO` & `rfcontrolpy-0.0.5/rfcontrolpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfcontrolpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library with protocol support for different 433MHz switches and weather stations for the RFControl Arduino library.
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/rfcontrolpy
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/rfcontrolpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `rfcontrolpy-0.0.4/rfcontrolpy.egg-info/SOURCES.txt` & `rfcontrolpy-0.0.5/rfcontrolpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 rfcontrol/py.typed
 rfcontrol/protocols/__init__.py
 rfcontrol/protocols/_skeleton.py
 rfcontrol/protocols/dimmer1.py
 rfcontrol/protocols/dimmer2.py
 rfcontrol/protocols/generic.py
 rfcontrol/protocols/generic2.py
+rfcontrol/protocols/pir1.py
+rfcontrol/protocols/pir2.py
 rfcontrol/protocols/pir3.py
+rfcontrol/protocols/pir6.py
 rfcontrol/protocols/switch1.py
 rfcontrol/protocols/switch10.py
 rfcontrol/protocols/switch11.py
 rfcontrol/protocols/switch2.py
 rfcontrol/protocols/switch25.py
 rfcontrol/protocols/switch3.py
 rfcontrol/protocols/switch4.py
```

### Comparing `rfcontrolpy-0.0.4/tests/test_controller.py` & `rfcontrolpy-0.0.5/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.4/tests/test_helpers.py` & `rfcontrolpy-0.0.5/tests/test_helpers.py`

 * *Files identical despite different names*

