# Comparing `tmp/pegasus-wms.api-5.0.5.tar.gz` & `tmp/pegasus-wms.api-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../../dist/pegasus-wms.api-5.0.5.tar", last modified: Fri Feb 17 18:24:04 2023, max compression
+gzip compressed data, was "pegasus-wms.api-5.0.6.tar", last modified: Mon Jul  3 15:44:36 2023, max compression
```

## Comparing `pegasus-wms.api-5.0.5.tar` & `pegasus-wms.api-5.0.6.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/Pegasus/
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/
--rw-r--r--   0 bamboo     (550) users      (100)      521 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/__init__.py
--rw-r--r--   0 bamboo     (550) users      (100)     2307 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/_utils.py
--rw-r--r--   0 bamboo     (550) users      (100)      133 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/errors.py
--rw-r--r--   0 bamboo     (550) users      (100)    38835 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/mixins.py
--rw-r--r--   0 bamboo     (550) users      (100)    10959 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/properties.py
--rw-r--r--   0 bamboo     (550) users      (100)    11737 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/replica_catalog.py
--rw-r--r--   0 bamboo     (550) users      (100)    18835 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/site_catalog.py
--rw-r--r--   0 bamboo     (550) users      (100)    31657 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/transformation_catalog.py
--rw-r--r--   0 bamboo     (550) users      (100)    79974 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/workflow.py
--rw-r--r--   0 bamboo     (550) users      (100)     6315 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/src/Pegasus/api/writable.py
-drwxr-xr-x   0 bamboo     (550) users      (100)        0 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/pegasus_wms.api.egg-info/
--rw-r--r--   0 bamboo     (550) users      (100)     1926 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/pegasus_wms.api.egg-info/PKG-INFO
--rw-r--r--   0 bamboo     (550) users      (100)      605 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/pegasus_wms.api.egg-info/SOURCES.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/pegasus_wms.api.egg-info/dependency_links.txt
--rw-r--r--   0 bamboo     (550) users      (100)        1 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/pegasus_wms.api.egg-info/not-zip-safe
--rw-r--r--   0 bamboo     (550) users      (100)       19 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/pegasus_wms.api.egg-info/requires.txt
--rw-r--r--   0 bamboo     (550) users      (100)        8 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/src/pegasus_wms.api.egg-info/top_level.txt
--rw-r--r--   0 bamboo     (550) users      (100)    11368 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/LICENSE
--rw-r--r--   0 bamboo     (550) users      (100)       60 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/MANIFEST.in
--rw-r--r--   0 bamboo     (550) users      (100)      425 2023-02-17 18:23:44.000000 pegasus-wms.api-5.0.5/README.md
--rw-r--r--   0 bamboo     (550) users      (100)      176 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/setup.cfg
--rw-r--r--   0 bamboo     (550) users      (100)     2701 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/setup.py
--rw-r--r--   0 bamboo     (550) users      (100)     1926 2023-02-17 18:24:04.000000 pegasus-wms.api-5.0.5/PKG-INFO
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:36.051364 pegasus-wms.api-5.0.6/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    11368 2023-06-30 20:04:01.000000 pegasus-wms.api-5.0.6/LICENSE
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       60 2023-07-03 15:42:39.000000 pegasus-wms.api-5.0.6/MANIFEST.in
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1805 2023-07-03 15:44:36.051364 pegasus-wms.api-5.0.6/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      425 2023-06-30 20:04:01.000000 pegasus-wms.api-5.0.6/README.md
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      615 2023-06-30 20:04:01.000000 pegasus-wms.api-5.0.6/pyproject.toml
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      176 2023-07-03 15:44:36.051364 pegasus-wms.api-5.0.6/setup.cfg
+-rw-------   0 rynge     (1000) rynge     (1000)     2701 2023-07-03 15:44:34.000000 pegasus-wms.api-5.0.6/setup.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:36.035364 pegasus-wms.api-5.0.6/src/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:36.035364 pegasus-wms.api-5.0.6/src/Pegasus/
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:36.047364 pegasus-wms.api-5.0.6/src/Pegasus/api/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      521 2023-06-30 20:04:01.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/__init__.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     2307 2023-06-30 20:04:01.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/_utils.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      133 2023-06-30 20:04:01.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/errors.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    39152 2023-07-03 15:42:39.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/mixins.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    10959 2023-07-03 15:42:39.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/properties.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    11752 2023-07-03 15:42:39.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/replica_catalog.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    18859 2023-07-03 15:42:39.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/site_catalog.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    31657 2023-07-03 15:42:39.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/transformation_catalog.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)    79999 2023-07-03 15:42:39.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/workflow.py
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     6315 2023-07-03 15:42:39.000000 pegasus-wms.api-5.0.6/src/Pegasus/api/writable.py
+drwxr-xr-x   0 rynge     (1000) rynge     (1000)        0 2023-07-03 15:44:36.051364 pegasus-wms.api-5.0.6/src/pegasus_wms.api.egg-info/
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1805 2023-07-03 15:44:35.000000 pegasus-wms.api-5.0.6/src/pegasus_wms.api.egg-info/PKG-INFO
+-rw-r--r--   0 rynge     (1000) rynge     (1000)      628 2023-07-03 15:44:35.000000 pegasus-wms.api-5.0.6/src/pegasus_wms.api.egg-info/SOURCES.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:35.000000 pegasus-wms.api-5.0.6/src/pegasus_wms.api.egg-info/dependency_links.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        1 2023-07-03 15:44:35.000000 pegasus-wms.api-5.0.6/src/pegasus_wms.api.egg-info/not-zip-safe
+-rw-r--r--   0 rynge     (1000) rynge     (1000)       19 2023-07-03 15:44:35.000000 pegasus-wms.api-5.0.6/src/pegasus_wms.api.egg-info/requires.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)        8 2023-07-03 15:44:35.000000 pegasus-wms.api-5.0.6/src/pegasus_wms.api.egg-info/top_level.txt
+-rw-r--r--   0 rynge     (1000) rynge     (1000)     1855 2023-07-03 15:42:39.000000 pegasus-wms.api-5.0.6/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pegasus-wms.api-5.0.5/src/Pegasus/api/__init__.py` & `pegasus-wms.api-5.0.6/src/Pegasus/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.api-5.0.5/src/Pegasus/api/_utils.py` & `pegasus-wms.api-5.0.6/src/Pegasus/api/_utils.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.api-5.0.5/src/Pegasus/api/mixins.py` & `pegasus-wms.api-5.0.6/src/Pegasus/api/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,26 @@
         raise ValueError(
             "value: {} should be a str formatted as '<int> [MB | GB | TB | PB | EB | ZB | YB]'".format(
                 value
             )
         )
 
 
+def to_kb(value: str) -> int:
+    """Convert the given value to KB
+
+    :param value: str formatted as str formatted as :code:`'<int> [MB | GB | TB | PB | EB | ZB | YB]'`
+    :type value: str
+    :raises ValueError: invalid format
+    :return: value in KB
+    :rtype: int
+    """
+    return to_mb(value) * 1024
+
+
 class ProfileMixin:
     @_chained
     def add_profiles(
         self,
         ns: Namespace,
         key: Optional[str] = None,
         value: Optional[Union[str, int, float, bool, Path]] = None,
@@ -356,15 +368,15 @@
         filesystem_domain="filesystemdomain",
         stream_error="stream_error",
         stream_output="stream_output",
         priority="priority",
         request_cpus="request_cpus",
         request_gpus="request_gpus",
         request_memory=("request_memory", to_mb),
-        request_disk=("request_disk", to_mb),
+        request_disk=("request_disk", to_kb),
         requirements="requirements",
         should_transfer_files="should_transfer_files",
         when_to_transfer_output="when_to_transfer_output",
         condor_collector="condor_collector",
         grid_resource="grid_resource",
         cream_attributes="cream_attributes",
     )
@@ -540,15 +552,15 @@
         :type clusters_num: int, optional
         :param clusters_size: Determines the number of jobs in each cluster (see `Pegasus Clustering Guide <https://pegasus.isi.edu/documentation/job_clustering.php#horizontal_clustering>`_ for more information), defaults to None
         :type clusters_size: int, optional
         :param job_aggregator: Indicates the clustering executable that is used to run the clustered job on the remote site, defaults to None
         :type job_aggregator: int, optional
         :param job_aggregator_arguments: Additional arguments with which a clustering executable should be invoked, defaults to None
         :type job_aggregator_arguments: str, optional
-        :param grid_start: Determines the executable for launching a job (see `docs <https://pegasus.isi.edu/documentation/profiles.php#hints_profiles>`_ for more information), defaults to None
+        :param grid_start: Determines the executable for launching a job (see `docs <https://pegasus.isi.edu/documentation/profiles.php#hints_profiles>`__ for more information), defaults to None
         :type grid_start: int, optional
         :param grid_start_path: Sets the path to the gridstart . This profile is best set in the Site Catalog, defaults to None
         :type grid_start_path: str, optional
         :param grid_start_arguments: Sets the arguments with which GridStart is used to launch a job on the remote site, defaults to None
         :type grid_start_arguments: str, optional
         :param grid_start_launcher: specifies the path to the executable to launch kickstart, defaults to None,
         :type grid_start_launcher: str, optional
@@ -654,15 +666,15 @@
         Mapper during site selection. This gives you finer grained control over
         where a job executes and what executable it refers to.
 
         :param execution_site: the execution site where a job should be executed, defaults to None
         :type execution_site: str, optional
         :param pfn: the physical file name to the main executable that a job refers to. Overrides any entries specified in the transformation catalog, defaults to None
         :type pfn: Union[str, Path], optional
-        :param grid_job_type: This profile is usually used to ensure that a compute job executes on another job manager (see `docs <https://pegasus.isi.edu/documentation/profiles.php#hints_profiles>`_ for more information), defaults to None
+        :param grid_job_type: This profile is usually used to ensure that a compute job executes on another job manager (see `docs <https://pegasus.isi.edu/documentation/profiles.php#hints_profiles>`__ for more information), defaults to None
         :type grid_job_type: str, optional
         :return: self
         """
         ...
 
     @_profiles(
         Namespace.DAGMAN,
@@ -707,15 +719,15 @@
             job.add_profiles(Namespace.DAGMAN, key="post.path.<value of dagman.post>", value=<value string>)
             job.add_profiles(Namespace.DAGMAN, key="<category-name>.maxjobs", value=<value string>)
 
         :param pre: is the path to the pre-script. DAGMan executes the pre-script before it runs the job, defaults to None
         :type pre: Union[str, Path], optional
         :param pre_arguments: are command-line arguments for the pre-script, if any, defaults to None
         :type pre_arguments: str, optional
-        :param post: is the postscript type/mode that a user wants to associate with a job (see `docs <https://pegasus.isi.edu/documentation/profiles.php>`_ for more information), defaults to None
+        :param post: is the postscript type/mode that a user wants to associate with a job (see `docs <https://pegasus.isi.edu/documentation/profiles.php>`__ for more information), defaults to None
         :type post: str, optional
         :param post_arguments: are the command line arguments for the post script, if any, defaults to None
         :type post_arguments: str, optional
         :param retry: is the number of times DAGMan retries the full job cycle from pre-script through post-script, if failure was detected, defaults to None
         :type retry: int, optional
         :param category: the DAGMan category the job belongs to, defaults to None
         :type category: str, optional
@@ -727,15 +739,15 @@
         :type max_pre: str, optional
         :param max_post: sets the maximum number of POST scripts within the DAG that may be running at one time, defaults to None
         :type max_post: str, optional
         :param max_jobs: sets the maximum number of jobs within the DAG that will be submitted to Condor at one time, defaults to None
         :type max_jobs: str, optional
         :param max_idle: Sets the maximum number of idle jobs allowed before HTCondor DAGMan stops submitting more jobs. Once idle jobs start to run, HTCondor DAGMan will resume submitting jobs. If the option is omitted, the number of idle jobs is unlimited, defaults to None
         :type max_idle: str, optional
-        :param post_scope: can be "all", "none" or "essential" (see `docs <https://pegasus.isi.edu/documentation/profiles.php>`_ for more information), defaults to None
+        :param post_scope: can be "all", "none" or "essential" (see `docs <https://pegasus.isi.edu/documentation/profiles.php>`__ for more information), defaults to None
         :type post_scope: str, optional
         :return: self
         """
         ...
 
     # initially had add_<namespace>_profile for 5.0 release and in order not not
     # break existing workflows, these functions have aliases that are plural
```

### Comparing `pegasus-wms.api-5.0.5/src/Pegasus/api/properties.py` & `pegasus-wms.api-5.0.6/src/Pegasus/api/properties.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.api-5.0.5/src/Pegasus/api/replica_catalog.py` & `pegasus-wms.api-5.0.6/src/Pegasus/api/replica_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,17 @@
     .. code-block:: python
 
         # Example
         input_file = File("data.txt").add_metadata(creator="ryan")
 
     """
 
-    def __init__(self, lfn: str, size: Optional[int] = None, for_planning: Optional[bool] = False):
+    def __init__(
+        self, lfn: str, size: Optional[int] = None, for_planning: Optional[bool] = False
+    ):
         """
         :param lfn: a unique logical filename
         :type lfn: str
         :param size: size in bytes, defaults to None
         :type size: int
         :param for_planning: indicate that a file is to be used for planning purposes
         :type for_planning: bool
@@ -87,15 +89,15 @@
     def __json__(self):
         return _filter_out_nones(
             OrderedDict(
                 [
                     ("lfn", self.lfn),
                     ("metadata", self.metadata if len(self.metadata) > 0 else None),
                     ("size", self.size),
-                    ("forPlanning", self.for_planning)
+                    ("forPlanning", self.for_planning),
                 ]
             )
         )
 
 
 class _ReplicaCatalogEntry:
     def __init__(
```

### Comparing `pegasus-wms.api-5.0.5/src/Pegasus/api/site_catalog.py` & `pegasus-wms.api-5.0.6/src/Pegasus/api/site_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     PPC = "ppc"
     PPC_64 = "ppc_64"
     PPC64LE = "ppc64le"
     IA64 = "ia64"
     SPARCV7 = "sparcv7"
     SPARCV9 = "sparcv9"
     AMD64 = "amd64"
+    AARCH64 = "aarch64"
 
 
 class OS(Enum):
     """Operating system types"""
 
     LINUX = "linux"
     SUNOS = "sunos"
```

### Comparing `pegasus-wms.api-5.0.5/src/Pegasus/api/transformation_catalog.py` & `pegasus-wms.api-5.0.6/src/Pegasus/api/transformation_catalog.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.api-5.0.5/src/Pegasus/api/workflow.py` & `pegasus-wms.api-5.0.6/src/Pegasus/api/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,15 +549,15 @@
             self.file = file
 
         # ensure that add_planner_args() is not invoked multiple times for each SubWorkflow
         # instance as this will create duplicate arguments
         self._planner_args_already_set = False
 
         if not isinstance(self.file, Workflow):
-            self.add_inputs(self.file)
+            self.add_inputs(File(self.file, for_planning=True))
 
     @_chained
     def add_planner_args(
         self,
         *,
         conf: Optional[Union[str, Path]] = None,
         basename: Optional[str] = None,
```

### Comparing `pegasus-wms.api-5.0.5/src/Pegasus/api/writable.py` & `pegasus-wms.api-5.0.6/src/Pegasus/api/writable.py`

 * *Files identical despite different names*

### Comparing `pegasus-wms.api-5.0.5/src/pegasus_wms.api.egg-info/PKG-INFO` & `pegasus-wms.api-5.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms.api
-Version: 5.0.5
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Python API
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
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,7 +25,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
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

### Comparing `pegasus-wms.api-5.0.5/src/pegasus_wms.api.egg-info/SOURCES.txt` & `pegasus-wms.api-5.0.6/src/pegasus_wms.api.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
+tox.ini
 src/Pegasus/api/__init__.py
 src/Pegasus/api/_utils.py
 src/Pegasus/api/errors.py
 src/Pegasus/api/mixins.py
 src/Pegasus/api/properties.py
 src/Pegasus/api/replica_catalog.py
 src/Pegasus/api/site_catalog.py
```

### Comparing `pegasus-wms.api-5.0.5/LICENSE` & `pegasus-wms.api-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pegasus-wms.api-5.0.5/setup.py` & `pegasus-wms.api-5.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             pkgs.append(os.path.join(root, pkg).replace("/", "."))
 
     return pkgs
 
 
 setup(
     name="pegasus-wms.api",
-    version="5.0.5",
+    version="5.0.6",
     author="Pegasus Team",
     author_email="pegasus@isi.edu",
     description="Pegasus Workflow Management System Python API",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     license="Apache2",
     url="http://pegasus.isi.edu",
```

### Comparing `pegasus-wms.api-5.0.5/PKG-INFO` & `pegasus-wms.api-5.0.6/src/pegasus_wms.api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 Metadata-Version: 2.1
 Name: pegasus-wms.api
-Version: 5.0.5
+Version: 5.0.6
 Summary: Pegasus Workflow Management System Python API
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
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,7 +25,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
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

