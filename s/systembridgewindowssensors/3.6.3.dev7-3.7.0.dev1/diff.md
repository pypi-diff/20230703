# Comparing `tmp/systembridgewindowssensors-3.6.3.dev7.tar.gz` & `tmp/systembridgewindowssensors-3.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgewindowssensors-3.6.3.dev7.tar", last modified: Thu Apr 13 20:22:51 2023, max compression
+gzip compressed data, was "systembridgewindowssensors-3.7.0.dev1.tar", last modified: Mon Jul  3 08:36:16 2023, max compression
```

## Comparing `systembridgewindowssensors-3.6.3.dev7.tar` & `systembridgewindowssensors-3.7.0.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:51.908687 systembridgewindowssensors-3.6.3.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-13 20:22:51.908687 systembridgewindowssensors-3.6.3.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-13 20:22:29.000000 systembridgewindowssensors-3.6.3.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:22:51.908687 systembridgewindowssensors-3.6.3.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-13 20:22:29.000000 systembridgewindowssensors-3.6.3.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:51.892686 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-13 20:22:29.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-13 20:22:49.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:51.908687 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   242608 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.dll
--rw-r--r--   0 runner    (1001) docker     (123)   589312 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    55484 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.xml
--rw-r--r--   0 runner    (1001) docker     (123)   716800 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/LibreHardwareMonitorLib.dll
--rw-r--r--   0 runner    (1001) docker     (123)   122070 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/LibreHardwareMonitorLib.xml
--rw-r--r--   0 runner    (1001) docker     (123)   701992 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/Newtonsoft.Json.dll
--rw-r--r--   0 runner    (1001) docker     (123)   468480 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/NvAPIWrapper.dll
--rw-r--r--   0 runner    (1001) docker     (123)  1033515 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/NvAPIWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (123)    30208 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-13 20:22:30.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:22:51.896687 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 20:22:51.000000 systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:36:16.420017 systembridgewindowssensors-3.7.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-03 08:36:16.416017 systembridgewindowssensors-3.7.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 08:35:50.000000 systembridgewindowssensors-3.7.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:36:16.420017 systembridgewindowssensors-3.7.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-03 08:35:50.000000 systembridgewindowssensors-3.7.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:36:16.408017 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 08:35:50.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-03 08:36:13.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:36:16.416017 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   242608 2023-07-03 08:35:51.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/HidSharp.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   589312 2023-07-03 08:35:51.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/HidSharp.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    55484 2023-07-03 08:35:51.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/HidSharp.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   716800 2023-07-03 08:35:51.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/LibreHardwareMonitorLib.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   122070 2023-07-03 08:35:51.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/LibreHardwareMonitorLib.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   701992 2023-07-03 08:35:51.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/Newtonsoft.Json.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   468480 2023-07-03 08:35:51.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/NvAPIWrapper.dll
+-rw-r--r--   0 runner    (1001) docker     (123)  1033515 2023-07-03 08:35:52.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/NvAPIWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    30208 2023-07-03 08:35:52.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-03 08:35:52.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:36:16.408017 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-03 08:36:16.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-03 08:36:16.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:36:16.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 08:36:16.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 08:36:16.000000 systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors.egg-info/top_level.txt
```

### Comparing `systembridgewindowssensors-3.6.3.dev7/pyproject.toml` & `systembridgewindowssensors-3.7.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/setup.py` & `systembridgewindowssensors-3.7.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.dll` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/HidSharp.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.pdb` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/HidSharp.pdb`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/HidSharp.xml` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/HidSharp.xml`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/LibreHardwareMonitorLib.dll` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/LibreHardwareMonitorLib.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/LibreHardwareMonitorLib.xml` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/LibreHardwareMonitorLib.xml`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/Newtonsoft.Json.dll` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/NvAPIWrapper.dll` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/NvAPIWrapper.dll`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/NvAPIWrapper.xml` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/NvAPIWrapper.xml`

 * *Files identical despite different names*

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors/bin/SystemBridgeWindowsSensors.exe`

 * *Files 4% similar despite different names*

#### pedump {}

```diff
@@ -1,12 +1,12 @@
 
 COFF Header:
 	                Machine: 0x8664
 	               Sections: 0x0002
-	             Time stamp: 0xba4543cf
+	             Time stamp: 0xa4307cb7
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00f0
 	   	Characteristics: 0x0022
 
 PE Header:
 	         Magic (0x010b): 0x020b
@@ -57,15 +57,15 @@
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00000000 [0x00000000]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002000 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00002ee1
+	   Virtual Size: 0x00002ede
 	Virtual Address: 0x00002000
 	  Raw Data Size: 0x00003000
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
```

### Comparing `systembridgewindowssensors-3.6.3.dev7/systembridgewindowssensors.egg-info/SOURCES.txt` & `systembridgewindowssensors-3.7.0.dev1/systembridgewindowssensors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

