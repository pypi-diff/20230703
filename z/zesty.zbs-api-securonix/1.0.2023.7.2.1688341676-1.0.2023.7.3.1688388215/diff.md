# Comparing `tmp/zesty.zbs-api-securonix-1.0.2023.7.2.1688341676.tar.gz` & `tmp/zesty.zbs-api-securonix-1.0.2023.7.3.1688388215.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.7.2.1688341676.tar", last modified: Sun Jul  2 23:47:57 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.7.3.1688388215.tar", last modified: Mon Jul  3 12:43:35 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676.tar` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1175 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14360 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     8818 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7367 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    16086 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    14309 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     7202 2023-07-02 23:47:00.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/zesty.zbs_api_securonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/zesty.zbs_api_securonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/zesty.zbs_api_securonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/zesty.zbs_api_securonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/zesty.zbs_api_securonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-02 23:47:57.000000 zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/zesty.zbs_api_securonix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14360 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7367 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16109 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    14309 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     7202 2023-07-03 12:43:11.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/zesty.zbs_api_securonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/zesty.zbs_api_securonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/zesty.zbs_api_securonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/zesty.zbs_api_securonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/zesty.zbs_api_securonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-03 12:43:35.000000 zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/zesty.zbs_api_securonix.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.7.2.1688341676
+Version: 1.0.2023.7.3.1688388215
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/README.md` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/setup.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/actions.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/FileSystem.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/ManagedFS.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,16 +285,17 @@
     reboot = Column(BOOLEAN, default=False)
     # array of day numbers when reboot is allowed 0-6
     days = Column(ARRAY(VARCHAR))
     # timeframe from-to in %I:%M %p
     from_ = Column(VARCHAR)
     to = Column(VARCHAR)
 
+    status = Column(VARCHAR, nullable=False, server_default="Active")
     is_rebooting = Column(BOOLEAN, default=False)
-    is_aborted = Column(BOOLEAN, default=False)
+
     # Snapshot and ebs deletion in days
     ebs_remove_after = Column(INT, nullable=True)
     snapshot_remove_after = Column(INT, nullable=True)
 
     def __init__(
             self,
             fs_id: str,
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/Usage.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/agent_report.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/disk_mon.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/hf_interface.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/models/overview.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/protocol.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/protocol.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/src/step_instructions.py` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/src/step_instructions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/zesty.zbs_api_securonix.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/zesty.zbs_api_securonix.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.7.2.1688341676
+Version: 1.0.2023.7.3.1688388215
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.7.2.1688341676/zesty.zbs_api_securonix.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-1.0.2023.7.3.1688388215/zesty.zbs_api_securonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

