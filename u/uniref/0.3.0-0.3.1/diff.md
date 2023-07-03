# Comparing `tmp/uniref-0.3.0.tar.gz` & `tmp/uniref-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniref-0.3.0.tar", last modified: Tue Mar 28 04:55:31 2023, max compression
+gzip compressed data, was "uniref-0.3.1.tar", last modified: Mon Jul  3 10:18:14 2023, max compression
```

## Comparing `uniref-0.3.0.tar` & `uniref-0.3.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.763203 uniref-0.3.0/
--rw-rw-rw-   0        0        0    34523 2023-02-13 01:03:22.000000 uniref-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    43695 2023-03-28 04:55:31.762202 uniref-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2251 2023-02-24 10:26:03.000000 uniref-0.3.0/README.md
--rw-rw-rw-   0        0        0     1188 2023-03-28 04:50:42.000000 uniref-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-28 04:55:31.763203 uniref-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.721208 uniref-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.729215 uniref-0.3.0/src/uniref/
--rw-rw-rw-   0        0        0       91 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.723209 uniref-0.3.0/src/uniref/bin/
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.735219 uniref-0.3.0/src/uniref/bin/android/
--rw-rw-rw-   0        0        0     5260 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/bin/android/agent.js
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.738446 uniref-0.3.0/src/uniref/bin/win/
--rwxrwxrwx   0        0        0     9216 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/bin/win/getproc32.exe
--rwxrwxrwx   0        0        0    10752 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/bin/win/getproc64.exe
--rw-rw-rw-   0        0        0    18944 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/bin/win/util64.dll
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.744453 uniref-0.3.0/src/uniref/define/
--rw-rw-rw-   0        0        0        0 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/define/__init__.py
--rw-rw-rw-   0        0        0     6784 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/define/constant.py
--rw-rw-rw-   0        0        0     1977 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/define/patch.py
--rw-rw-rw-   0        0        0     1773 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/define/struct.py
--rw-rw-rw-   0        0        0    18119 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/define/types.py
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.747188 uniref-0.3.0/src/uniref/mono/
--rw-rw-rw-   0        0        0        0 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/mono/__init__.py
--rw-rw-rw-   0        0        0    21129 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/mono/assets.py
--rw-rw-rw-   0        0        0    25004 2023-03-28 03:51:18.000000 uniref-0.3.0/src/uniref/mono/component.py
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.751192 uniref-0.3.0/src/uniref/mono/injector/
--rw-rw-rw-   0        0        0       78 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/mono/injector/__init__.py
--rw-rw-rw-   0        0        0     3697 2023-03-28 04:14:08.000000 uniref-0.3.0/src/uniref/mono/injector/android.py
--rw-rw-rw-   0        0        0    22312 2023-03-28 04:13:39.000000 uniref-0.3.0/src/uniref/mono/injector/interface.py
--rw-rw-rw-   0        0        0     5269 2023-03-28 04:12:07.000000 uniref-0.3.0/src/uniref/mono/injector/windows.py
--rw-rw-rw-   0        0        0     8436 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/platforms.py
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.757197 uniref-0.3.0/src/uniref/util/
--rw-rw-rw-   0        0        0        0 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/util/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/util/compiler.py
--rw-rw-rw-   0        0        0      690 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/util/disasm.py
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.761201 uniref-0.3.0/src/uniref/util/injector/
--rw-rw-rw-   0        0        0       70 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/util/injector/__init__.py
--rw-rw-rw-   0        0        0    12062 2023-03-28 03:37:13.000000 uniref-0.3.0/src/uniref/util/injector/android.py
--rw-rw-rw-   0        0        0    25310 2023-03-28 03:37:03.000000 uniref-0.3.0/src/uniref/util/injector/interface.py
--rw-rw-rw-   0        0        0    18951 2023-03-28 04:24:09.000000 uniref-0.3.0/src/uniref/util/injector/windows.py
--rw-rw-rw-   0        0        0     8535 2023-02-13 01:03:23.000000 uniref-0.3.0/src/uniref/util/scanner.py
--rw-rw-rw-   0        0        0     8175 2023-03-06 11:26:00.000000 uniref-0.3.0/src/uniref/util/winapi.py
-drwxrwxrwx   0        0        0        0 2023-03-28 04:55:31.734219 uniref-0.3.0/src/uniref.egg-info/
--rw-rw-rw-   0        0        0    43695 2023-03-28 04:55:31.000000 uniref-0.3.0/src/uniref.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1030 2023-03-28 04:55:31.000000 uniref-0.3.0/src/uniref.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 04:55:31.000000 uniref-0.3.0/src/uniref.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-03-28 04:55:31.000000 uniref-0.3.0/src/uniref.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-28 04:55:31.000000 uniref-0.3.0/src/uniref.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.482679 uniref-0.3.1/
+-rw-rw-rw-   0        0        0    34523 2023-02-13 01:03:22.000000 uniref-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0    43695 2023-07-03 10:18:14.482679 uniref-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2251 2023-02-24 10:26:03.000000 uniref-0.3.1/README.md
+-rw-rw-rw-   0        0        0     1188 2023-07-03 10:17:03.000000 uniref-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 10:18:14.482679 uniref-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.437515 uniref-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.446524 uniref-0.3.1/src/uniref/
+-rw-rw-rw-   0        0        0       91 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.438516 uniref-0.3.1/src/uniref/bin/
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.453529 uniref-0.3.1/src/uniref/bin/android/
+-rw-rw-rw-   0        0        0     5260 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/bin/android/agent.js
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.456532 uniref-0.3.1/src/uniref/bin/win/
+-rwxrwxrwx   0        0        0     9216 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/bin/win/getproc32.exe
+-rwxrwxrwx   0        0        0    10752 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/bin/win/getproc64.exe
+-rw-rw-rw-   0        0        0    18944 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/bin/win/util64.dll
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.462538 uniref-0.3.1/src/uniref/define/
+-rw-rw-rw-   0        0        0        0 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/define/__init__.py
+-rw-rw-rw-   0        0        0     6784 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/define/constant.py
+-rw-rw-rw-   0        0        0     1977 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/define/patch.py
+-rw-rw-rw-   0        0        0     1773 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/define/struct.py
+-rw-rw-rw-   0        0        0    18119 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/define/types.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.465541 uniref-0.3.1/src/uniref/mono/
+-rw-rw-rw-   0        0        0        0 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/mono/__init__.py
+-rw-rw-rw-   0        0        0    21129 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/mono/assets.py
+-rw-rw-rw-   0        0        0    25004 2023-03-28 03:51:18.000000 uniref-0.3.1/src/uniref/mono/component.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.470545 uniref-0.3.1/src/uniref/mono/injector/
+-rw-rw-rw-   0        0        0       78 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/mono/injector/__init__.py
+-rw-rw-rw-   0        0        0     3697 2023-03-28 04:14:08.000000 uniref-0.3.1/src/uniref/mono/injector/android.py
+-rw-rw-rw-   0        0        0    22312 2023-03-28 04:13:39.000000 uniref-0.3.1/src/uniref/mono/injector/interface.py
+-rw-rw-rw-   0        0        0     5315 2023-07-03 10:00:32.000000 uniref-0.3.1/src/uniref/mono/injector/windows.py
+-rw-rw-rw-   0        0        0     8436 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/platforms.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.475550 uniref-0.3.1/src/uniref/util/
+-rw-rw-rw-   0        0        0        0 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/util/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/util/compiler.py
+-rw-rw-rw-   0        0        0      690 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/util/disasm.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.480554 uniref-0.3.1/src/uniref/util/injector/
+-rw-rw-rw-   0        0        0       70 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/util/injector/__init__.py
+-rw-rw-rw-   0        0        0    12062 2023-03-28 03:37:13.000000 uniref-0.3.1/src/uniref/util/injector/android.py
+-rw-rw-rw-   0        0        0    25310 2023-03-28 03:37:03.000000 uniref-0.3.1/src/uniref/util/injector/interface.py
+-rw-rw-rw-   0        0        0    18951 2023-03-28 04:24:09.000000 uniref-0.3.1/src/uniref/util/injector/windows.py
+-rw-rw-rw-   0        0        0     8535 2023-02-13 01:03:23.000000 uniref-0.3.1/src/uniref/util/scanner.py
+-rw-rw-rw-   0        0        0     8175 2023-03-06 11:26:00.000000 uniref-0.3.1/src/uniref/util/winapi.py
+drwxrwxrwx   0        0        0        0 2023-07-03 10:18:14.452528 uniref-0.3.1/src/uniref.egg-info/
+-rw-rw-rw-   0        0        0    43695 2023-07-03 10:18:14.000000 uniref-0.3.1/src/uniref.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1030 2023-07-03 10:18:14.000000 uniref-0.3.1/src/uniref.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 10:18:14.000000 uniref-0.3.1/src/uniref.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-03 10:18:14.000000 uniref-0.3.1/src/uniref.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 10:18:14.000000 uniref-0.3.1/src/uniref.egg-info/top_level.txt
```

### Comparing `uniref-0.3.0/LICENSE` & `uniref-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/PKG-INFO` & `uniref-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniref
-Version: 0.3.0
+Version: 0.3.1
 Summary: Unity reflection framework
 Author-email: in1t <in1t@foxmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `uniref-0.3.0/README.md` & `uniref-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/pyproject.toml` & `uniref-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uniref"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="in1t", email="in1t@foxmail.com" },
 ]
 description = "Unity reflection framework"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

### Comparing `uniref-0.3.0/src/uniref/bin/android/agent.js` & `uniref-0.3.1/src/uniref/bin/android/agent.js`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/bin/win/getproc32.exe` & `uniref-0.3.1/src/uniref/bin/win/getproc32.exe`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/bin/win/getproc64.exe` & `uniref-0.3.1/src/uniref/bin/win/getproc64.exe`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/bin/win/util64.dll` & `uniref-0.3.1/src/uniref/bin/win/util64.dll`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/define/constant.py` & `uniref-0.3.1/src/uniref/define/constant.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/define/patch.py` & `uniref-0.3.1/src/uniref/define/patch.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/define/struct.py` & `uniref-0.3.1/src/uniref/define/struct.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/define/types.py` & `uniref-0.3.1/src/uniref/define/types.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/mono/assets.py` & `uniref-0.3.1/src/uniref/mono/assets.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/mono/component.py` & `uniref-0.3.1/src/uniref/mono/component.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/mono/injector/android.py` & `uniref-0.3.1/src/uniref/mono/injector/android.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/mono/injector/interface.py` & `uniref-0.3.1/src/uniref/mono/injector/interface.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/mono/injector/windows.py` & `uniref-0.3.1/src/uniref/mono/injector/windows.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return self._use_il2cpp
 
     @property
     def root_domain(self) -> int:
         return self._root_domain
 
     def _mono_detect(self) -> None:
-        h_mono = self.get_module_base("mono.dll")
+        h_mono = self.get_module_base("mono.dll") or self.get_module_base("mono-2.0-bdwgc.dll")
         if h_mono:
             self._h_mono = h_mono
         else:
             modules = WinApi.GetRemoteModules(self._h_process)
             for module in modules:
                 if self.get_proc_address(module, "il2cpp_thread_attach"):
                     self._h_mono = module
```

### Comparing `uniref-0.3.0/src/uniref/platforms.py` & `uniref-0.3.1/src/uniref/platforms.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/util/compiler.py` & `uniref-0.3.1/src/uniref/util/compiler.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/util/disasm.py` & `uniref-0.3.1/src/uniref/util/disasm.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/util/injector/android.py` & `uniref-0.3.1/src/uniref/util/injector/android.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/util/injector/interface.py` & `uniref-0.3.1/src/uniref/util/injector/interface.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/util/injector/windows.py` & `uniref-0.3.1/src/uniref/util/injector/windows.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/util/scanner.py` & `uniref-0.3.1/src/uniref/util/scanner.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref/util/winapi.py` & `uniref-0.3.1/src/uniref/util/winapi.py`

 * *Files identical despite different names*

### Comparing `uniref-0.3.0/src/uniref.egg-info/PKG-INFO` & `uniref-0.3.1/src/uniref.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniref
-Version: 0.3.0
+Version: 0.3.1
 Summary: Unity reflection framework
 Author-email: in1t <in1t@foxmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `uniref-0.3.0/src/uniref.egg-info/SOURCES.txt` & `uniref-0.3.1/src/uniref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

