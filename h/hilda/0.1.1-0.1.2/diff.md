# Comparing `tmp/hilda-0.1.1.tar.gz` & `tmp/hilda-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilda-0.1.1.tar", last modified: Wed Dec 21 06:09:35 2022, max compression
+gzip compressed data, was "hilda-0.1.2.tar", last modified: Mon Jul  3 14:30:55 2023, max compression
```

## Comparing `hilda-0.1.1.tar` & `hilda-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:35.246437 hilda-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2022-12-21 06:09:35.246437 hilda-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18368 2022-12-21 06:09:25.000000 hilda-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:35.242437 hilda-0.1.1/hilda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/from_ns_to_json.m
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/get_objectivec_class_description.m
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/get_objectivec_symbol_data.m
--rw-r--r--   0 runner    (1001) docker     (123)   120119 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/hilda_ascii_art.html
--rw-r--r--   0 runner    (1001) docker     (123)    40886 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/hilda_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/launch_lldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/lldb_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/lsof.m
--rw-r--r--   0 runner    (1001) docker     (123)    11366 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:35.246437 hilda-0.1.1/hilda/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/dyld.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/fs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:35.246437 hilda-0.1.1/hilda/snippets/mach/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/mach/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:35.246437 hilda-0.1.1/hilda/snippets/macho/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/macho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/macho/all_image_infos.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/macho/apple_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/macho/image_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/macho/macho.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/macho/macho_load_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/snippets/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2022-12-21 06:09:25.000000 hilda-0.1.1/hilda/to_ns_from_json.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:35.246437 hilda-0.1.1/hilda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2022-12-21 06:09:35.000000 hilda-0.1.1/hilda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2022-12-21 06:09:35.000000 hilda-0.1.1/hilda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 06:09:35.000000 hilda-0.1.1/hilda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-21 06:09:35.000000 hilda-0.1.1/hilda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-21 06:09:35.000000 hilda-0.1.1/hilda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-21 06:09:35.000000 hilda-0.1.1/hilda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      883 2022-12-21 06:09:35.246437 hilda-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 06:09:25.000000 hilda-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:35.246437 hilda-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 06:09:25.000000 hilda-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-21 06:09:25.000000 hilda-0.1.1/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2022-12-21 06:09:25.000000 hilda-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2022-12-21 06:09:25.000000 hilda-0.1.1/tests/hilda_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2022-12-21 06:09:25.000000 hilda-0.1.1/tests/lldb_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-07-03 14:30:55.881790 hilda-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-07-03 14:30:43.000000 hilda-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.877790 hilda-0.1.2/hilda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/from_ns_to_json.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/get_objectivec_class_description.m
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/get_objectivec_symbol_data.m
+-rw-r--r--   0 runner    (1001) docker     (123)   120119 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/hilda_ascii_art.html
+-rw-r--r--   0 runner    (1001) docker     (123)    40937 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/hilda_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/launch_lldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/lldb_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/lsof.m
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/hilda/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/dyld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/fs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/hilda/snippets/mach/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/mach/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/hilda/snippets/macho/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/all_image_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/apple_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/macho_load_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/remotepairingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/to_ns_from_json.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.877790 hilda-0.1.2/hilda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 14:30:55.885790 hilda-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:30:43.000000 hilda-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/hilda_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/lldb_entrypoint.py
```

### Comparing `hilda-0.1.1/PKG-INFO` & `hilda-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 0.1.1
+Version: 0.1.2
 Summary: LLDB wrapped and empowered by iPython's features
 Home-page: https://github.com/doronz88/hilda
 Author: DoronZ
 Project-URL: hilda, https://github.com/doronz88/hilda
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hilda-0.1.1/README.md` & `hilda-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/command.py` & `hilda-0.1.2/hilda/command.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/exceptions.py` & `hilda-0.1.2/hilda/exceptions.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/from_ns_to_json.m` & `hilda-0.1.2/hilda/from_ns_to_json.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/get_objectivec_class_description.m` & `hilda-0.1.2/hilda/get_objectivec_class_description.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/get_objectivec_symbol_data.m` & `hilda-0.1.2/hilda/get_objectivec_symbol_data.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/hilda_ascii_art.html` & `hilda-0.1.2/hilda/hilda_ascii_art.html`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/hilda_client.py` & `hilda-0.1.2/hilda/hilda_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,21 +235,24 @@
 
         if not err.Success():
             raise AccessingMemoryError()
 
         return retval
 
     @command()
-    def peek(self, address, size) -> bytes:
+    def peek(self, address, size: int) -> bytes:
         """
         Read data at given address
         :param address:
         :param size:
         :return:
         """
+        if size == 0:
+            return b''
+
         err = lldb.SBError()
         retval = self.process.ReadMemory(address, int(size), err)
 
         if not err.Success():
             raise AccessingMemoryError()
 
         return retval
```

### Comparing `hilda-0.1.1/hilda/launch_lldb.py` & `hilda-0.1.2/hilda/launch_lldb.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/lldb_entrypoint.py` & `hilda-0.1.2/hilda/lldb_entrypoint.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/lsof.m` & `hilda-0.1.2/hilda/lsof.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/objective_c_class.py` & `hilda-0.1.2/hilda/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/objective_c_symbol.py` & `hilda-0.1.2/hilda/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/registers.py` & `hilda-0.1.2/hilda/registers.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/snippets/dyld.py` & `hilda-0.1.2/hilda/snippets/dyld.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/snippets/macho/all_image_infos.py` & `hilda-0.1.2/hilda/snippets/macho/all_image_infos.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/snippets/macho/image_info.py` & `hilda-0.1.2/hilda/snippets/macho/image_info.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/snippets/macho/macho.py` & `hilda-0.1.2/hilda/snippets/macho/macho.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/snippets/macho/macho_load_commands.py` & `hilda-0.1.2/hilda/snippets/macho/macho_load_commands.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/snippets/xpc.py` & `hilda-0.1.2/hilda/snippets/xpc.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/symbol.py` & `hilda-0.1.2/hilda/symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/symbols_jar.py` & `hilda-0.1.2/hilda/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda/to_ns_from_json.m` & `hilda-0.1.2/hilda/to_ns_from_json.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/hilda.egg-info/PKG-INFO` & `hilda-0.1.2/hilda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 0.1.1
+Version: 0.1.2
 Summary: LLDB wrapped and empowered by iPython's features
 Home-page: https://github.com/doronz88/hilda
 Author: DoronZ
 Project-URL: hilda, https://github.com/doronz88/hilda
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `hilda-0.1.1/hilda.egg-info/SOURCES.txt` & `hilda-0.1.2/hilda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 hilda.egg-info/entry_points.txt
 hilda.egg-info/requires.txt
 hilda.egg-info/top_level.txt
 hilda/snippets/__init__.py
 hilda/snippets/collections.py
 hilda/snippets/dyld.py
 hilda/snippets/fs_utils.py
+hilda/snippets/remotepairingd.py
 hilda/snippets/syslog.py
 hilda/snippets/uuid.py
 hilda/snippets/xpc.py
 hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
 hilda/snippets/mach/__init__.py
 hilda/snippets/macho/__init__.py
 hilda/snippets/macho/all_image_infos.py
```

### Comparing `hilda-0.1.1/setup.cfg` & `hilda-0.1.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hilda
-version = 0.1.1
+version = 0.1.2
 description = LLDB wrapped and empowered by iPython's features
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = DoronZ
 classifiers = 
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
@@ -24,14 +24,15 @@
 	hexdump
 	ipython
 	click
 	objc_types_decoder
 	construct
 	pymobiledevice3
 	cached-property
+	keystone-engine
 
 [options.package_data]
 hilda = 
 	*.html
 	*.m
 
 [options.extras_require]
```

### Comparing `hilda-0.1.1/tests/conftest.py` & `hilda-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/tests/hilda_tests.py` & `hilda-0.1.2/tests/hilda_tests.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.1/tests/lldb_entrypoint.py` & `hilda-0.1.2/tests/lldb_entrypoint.py`

 * *Files identical despite different names*

