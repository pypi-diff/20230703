# Comparing `tmp/pegasus-wms.worker-5.0.5.tar.gz` & `tmp/pegasus-wms.worker-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../../dist/pegasus-wms.worker-5.0.5.tar", last modified: Fri Feb 17 18:24:05 2023, max compression
+gzip compressed data, was "pegasus-wms.worker-5.0.6.tar", last modified: Mon Jul  3 15:44:40 2023, max compression
```

## Comparing `pegasus-wms.worker-5.0.5.tar` & `pegasus-wms.worker-5.0.6.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/Pegasus/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/Pegasus/cli/
--rw-r--r--   0 bamboo     (550) users      (100)       65 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/cli/__init__.py
--rwxr-xr-x   0 bamboo     (550) users      (100)     2321 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-globus-online-init.py
--rwxr-xr-x   0 bamboo     (550) users      (100)    12129 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-globus-online.py
--rw-r--r--   0 bamboo     (550) users      (100)    16002 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-integrity.py
--rw-r--r--   0 bamboo     (550) users      (100)      743 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-s3.py
--rw-r--r--   0 bamboo     (550) users      (100)   182584 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-transfer.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/Pegasus/tools/
--rw-r--r--   0 bamboo     (550) users      (100)       65 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/tools/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)    11159 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/tools/worker_utils.py
--rw-r--r--   0 bamboo     (550) users      (100)       65 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/__init__.py
--rwxr-xr-x   0 bamboo     (550) users      (100)    28547 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/src/Pegasus/s3.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/pegasus_wms.worker.egg-info/
--rw-r--r--   0 bamboo     (550) users      (100)     2071 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/pegasus_wms.worker.egg-info/PKG-INFO
--rw-r--r--   0 bamboo     (550) users      (100)      646 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/pegasus_wms.worker.egg-info/SOURCES.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/pegasus_wms.worker.egg-info/dependency_links.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/pegasus_wms.worker.egg-info/not-zip-safe
--rw-r--r--   0 bamboo     (550) users      (100)       68 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/pegasus_wms.worker.egg-info/requires.txt
--rw-r--r--   0 bamboo     (550) users      (100)        8 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/src/pegasus_wms.worker.egg-info/top_level.txt
--rw-r--r--   0 bamboo     (550) users      (100)    11368 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/LICENSE
--rw-r--r--   0 bamboo     (550) users      (100)       60 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/MANIFEST.in
--rw-r--r--   0 bamboo     (550) users      (100)      425 2023-02-17 18:23:44.000000 pegasus-wms.worker-5.0.5/README.md
--rw-r--r--   0 bamboo     (550) users      (100)      176 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/setup.cfg
--rw-r--r--   0 bamboo     (550) users      (100)     2471 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/setup.py
--rw-r--r--   0 bamboo     (550) users      (100)     2071 2023-02-17 18:24:05.000000 pegasus-wms.worker-5.0.5/PKG-INFO
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:40.359412 pegasus-wms.worker-5.0.6/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    11368 2023-06-30 20:04:01.000000 pegasus-wms.worker-5.0.6/LICENSE
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       60 2023-07-03 15:42:39.000000 pegasus-wms.worker-5.0.6/MANIFEST.in
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1950 2023-07-03 15:44:40.359412 pegasus-wms.worker-5.0.6/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      425 2023-06-30 20:04:01.000000 pegasus-wms.worker-5.0.6/README.md
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      750 2023-07-03 15:42:39.000000 pegasus-wms.worker-5.0.6/pyproject.toml
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      176 2023-07-03 15:44:40.359412 pegasus-wms.worker-5.0.6/setup.cfg
+-rw-------   0 rynge     (1000) rynge     (1000)     2471 2023-07-03 15:44:39.000000 pegasus-wms.worker-5.0.6/setup.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:40.347412 pegasus-wms.worker-5.0.6/src/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:40.355412 pegasus-wms.worker-5.0.6/src/Pegasus/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       65 2023-06-30 20:04:01.000000 pegasus-wms.worker-5.0.6/src/Pegasus/__init__.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:40.355412 pegasus-wms.worker-5.0.6/src/Pegasus/cli/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       65 2023-06-30 20:04:01.000000 pegasus-wms.worker-5.0.6/src/Pegasus/cli/__init__.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)     2321 2023-07-03 15:42:39.000000 pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-globus-online-init.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)    12129 2023-06-30 20:04:01.000000 pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-globus-online.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    16002 2023-07-03 15:42:39.000000 pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-integrity.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      743 2023-06-30 20:04:01.000000 pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-s3.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)   183604 2023-07-03 15:42:39.000000 pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-transfer.py
+-rwxr-xr-x   0 rynge     (1000) rynge     (1000)    28547 2023-07-03 15:42:39.000000 pegasus-wms.worker-5.0.6/src/Pegasus/s3.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:40.359412 pegasus-wms.worker-5.0.6/src/Pegasus/tools/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       65 2023-06-30 20:04:01.000000 pegasus-wms.worker-5.0.6/src/Pegasus/tools/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    11159 2023-07-03 15:42:39.000000 pegasus-wms.worker-5.0.6/src/Pegasus/tools/worker_utils.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:40.359412 pegasus-wms.worker-5.0.6/src/pegasus_wms.worker.egg-info/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1950 2023-07-03 15:44:39.000000 pegasus-wms.worker-5.0.6/src/pegasus_wms.worker.egg-info/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      669 2023-07-03 15:44:40.000000 pegasus-wms.worker-5.0.6/src/pegasus_wms.worker.egg-info/SOURCES.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:39.000000 pegasus-wms.worker-5.0.6/src/pegasus_wms.worker.egg-info/dependency_links.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:39.000000 pegasus-wms.worker-5.0.6/src/pegasus_wms.worker.egg-info/not-zip-safe
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       68 2023-07-03 15:44:39.000000 pegasus-wms.worker-5.0.6/src/pegasus_wms.worker.egg-info/requires.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        8 2023-07-03 15:44:39.000000 pegasus-wms.worker-5.0.6/src/pegasus_wms.worker.egg-info/top_level.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1626 2023-07-03 15:42:39.000000 pegasus-wms.worker-5.0.6/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-globus-online-init.py` & `pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-globus-online-init.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-globus-online.py` & `pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-globus-online.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-integrity.py` & `pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-integrity.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-s3.py` & `pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-s3.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.worker-5.0.5/src/Pegasus/cli/pegasus-transfer.py` & `pegasus-wms.worker-5.0.6/src/Pegasus/cli/pegasus-transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3356,16 +3356,16 @@
 
 class StashHandler(TransferHandlerBase):
     """
     Uses the OSG stashcp command to trasfer from/to stash
     """
 
     _name = "StashHandler"
-    _mkdir_cleanup_protocols = ["stash"]
-    _protocol_map = ["stash->file", "file->stash"]
+    _mkdir_cleanup_protocols = ["osdf", "stash"]
+    _protocol_map = ["osdf->file", "stash->file", "file->osdf", "file->stash"]
 
     def do_mkdirs(self, transfers):
 
         # noop for now
         return [transfers, []]
 
         tools = utils.Tools()
@@ -3407,58 +3407,77 @@
 
         successful_l = []
         failed_l = []
         for t in transfers_l:
             self._pre_transfer_attempt(t)
             t_start = time.time()
 
-            if t.get_dst_proto() == "stash":
-                # write file:// to stash://
+            if t.get_dst_proto() in ["osdf", "stash"]:
+                # write file:// to osdf:// or stash://
 
                 # src has to exist and be readable
                 if not verify_local_file(t.get_src_path()):
                     self._post_transfer_attempt(t, False, t_start)
                     failed_l.append(t)
                     continue
 
-                if os.path.exists("/mnt/ceph/osg/public"):
-                    # hack for now - local cp
+                if os.path.exists("/mnt/stash/ospool"):
+                    # uw.osg-htc.org hack for now (we don't have a scitoken
+                    # locally) local cp
+                    src_path = t.get_src_path()
+                    dst_path = re.sub("^/ospool", "/mnt/stash/ospool", t.get_dst_path())
+
+                    prepare_local_dir(os.path.dirname(dst_path))
+                    cmd = "/bin/cp '%s' '%s'" % (src_path, dst_path)
+                elif os.path.exists("/mnt/ceph/osg"):
+                    # OSG Connect hack for now (we don't have a scitoken
+                    # locally) local cp
                     src_path = t.get_src_path()
                     dst_path = re.sub("^/osgconnect", "", t.get_dst_path())
 
                     prepare_local_dir(os.path.dirname(dst_path))
                     cmd = "/bin/cp '%s' '%s'" % (src_path, dst_path)
                 else:
                     cmd = "%s '%s' '%s'" % (
                         tools.full_path("stashcp"),
                         t.get_src_path(),
                         t.dst_url(),
                     )
             else:
                 # read
-                # stashcp wants just the path with a single leading slash
-                src_path = t.src_url()
-                src_path = re.sub("^stash:", "", src_path)
-                src_path = re.sub("^/+", "", src_path)
-                src_path = "/" + src_path
-
-                local_dir = os.path.dirname(t.get_dst_path())
-                prepare_local_dir(local_dir)
-                # use --methods as we want to exclude cvmfs - it can take a
-                # long time to update, and we have seen partial files being
-                # published there in the past
-                cmd = "%s '%s' '%s'" % (
-                    tools.full_path("stashcp"),
-                    src_path,
-                    local_dir,
-                )
-                remote_fname = os.path.basename(t.get_src_path())
-                local_fname = os.path.basename(t.get_dst_path())
-                if remote_fname != local_fname:
-                    cmd += " && mv '%s' '%s'" % (remote_fname, local_fname)
+
+                if os.path.exists("/mnt/stash/ospool"):
+                    # uw.osg-htc.org hack for now (we don't have a scitoken
+                    # locally) local cp
+                    src_path = re.sub("^/ospool", "/mnt/stash/ospool", t.get_src_path())
+                    dst_path = t.get_dst_path()
+
+                    prepare_local_dir(os.path.dirname(dst_path))
+                    cmd = "/bin/cp '%s' '%s'" % (src_path, dst_path)
+                elif os.path.exists("/mnt/ceph/osg"):
+                    # OSG Connect hack for now (we don't have a scitoken
+                    # locally) local cp
+                    src_path = re.sub("^/osgconnect", "", t.get_src_path())
+                    dst_path = t.get_dst_path()
+
+                    prepare_local_dir(os.path.dirname(dst_path))
+                    cmd = "/bin/cp '%s' '%s'" % (src_path, dst_path)
+                else:
+                    # stashcp wants just the path with a single leading slash
+                    src_path = t.src_url()
+                    src_path = re.sub("^(osdf|stash):", "", src_path)
+                    src_path = re.sub("^/+", "/", src_path)
+
+                    local_dir = os.path.dirname(t.get_dst_path())
+                    prepare_local_dir(local_dir)
+                    cmd = "%s '%s' '%s'" % (
+                        tools.full_path("stashcp"),
+                        src_path,
+                        t.get_dst_path(),
+                    )
 
             try:
                 tc = utils.TimedCommand(cmd)
                 tc.run()
             except RuntimeError as err:
                 logger.error(err)
                 self._post_transfer_attempt(t, False, t_start)
```

### Comparing `pegasus-wms.worker-5.0.5/src/Pegasus/tools/worker_utils.py` & `pegasus-wms.worker-5.0.6/src/Pegasus/tools/worker_utils.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.worker-5.0.5/src/Pegasus/s3.py` & `pegasus-wms.worker-5.0.6/src/Pegasus/s3.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.worker-5.0.5/src/pegasus_wms.worker.egg-info/PKG-INFO` & `pegasus-wms.worker-5.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms.worker
-Version: 5.0.5
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Worker Package Tools
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
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
@@ -43,7 +27,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=2.6,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
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

### Comparing `pegasus-wms.worker-5.0.5/src/pegasus_wms.worker.egg-info/SOURCES.txt` & `pegasus-wms.worker-5.0.6/src/pegasus_wms.worker.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
+tox.ini
 src/Pegasus/__init__.py
 src/Pegasus/s3.py
 src/Pegasus/cli/__init__.py
 src/Pegasus/cli/pegasus-globus-online-init.py
 src/Pegasus/cli/pegasus-globus-online.py
 src/Pegasus/cli/pegasus-integrity.py
 src/Pegasus/cli/pegasus-s3.py
```

### Comparing `pegasus-wms.worker-5.0.5/LICENSE` & `pegasus-wms.worker-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasus-wms.worker-5.0.5/setup.py` & `pegasus-wms.worker-5.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 #
 def read(fname):
     return open(os.path.join(src_dir, fname)).read()
 
 
 setup(
     name="pegasus-wms.worker",
-    version="5.0.5",
+    version="5.0.6",
     author="Pegasus Team",
     author_email="pegasus@isi.edu",
     description="Pegasus Workflow Management System Worker Package Tools",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     license="Apache2",
     url="http://pegasus.isi.edu",
```

### Comparing `pegasus-wms.worker-5.0.5/PKG-INFO` & `pegasus-wms.worker-5.0.6/src/pegasus_wms.worker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms.worker
-Version: 5.0.5
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Worker Package Tools
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
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
@@ -43,7 +27,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=2.6,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
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

