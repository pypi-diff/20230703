# Comparing `tmp/mypy-boto3-batch-1.26.98.tar.gz` & `tmp/mypy-boto3-batch-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-batch-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
+gzip compressed data, was "mypy-boto3-batch-1.27.0.tar", last modified: Mon Jul  3 19:50:25 2023, max compression
```

## Comparing `mypy-boto3-batch-1.26.98.tar` & `mypy-boto3-batch-1.27.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.399627 mypy-boto3-batch-1.26.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-03-23 19:33:04.387626 mypy-boto3-batch-1.26.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.383626 mypy-boto3-batch-1.26.98/mypy_boto3_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20489 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-03-23 19:31:56.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-03-23 19:31:56.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43981 2023-03-23 19:31:57.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43924 2023-03-23 19:31:57.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.387626 mypy-boto3-batch-1.26.98/mypy_boto3_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-03-23 19:33:04.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-23 19:33:04.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-23 19:33:04.000000 mypy-boto3-batch-1.26.98/mypy_boto3_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.399627 mypy-boto3-batch-1.26.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-23 19:31:55.000000 mypy-boto3-batch-1.26.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:25.958883 mypy-boto3-batch-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-03 19:50:25.958883 mypy-boto3-batch-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:25.958883 mypy-boto3-batch-1.27.0/mypy_boto3_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20489 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-03 19:33:07.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-03 19:33:07.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44362 2023-07-03 19:33:08.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44305 2023-07-03 19:33:07.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:25.958883 mypy-boto3-batch-1.27.0/mypy_boto3_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-03 19:50:25.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 19:50:25.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:25.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:25.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:25.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:50:25.000000 mypy-boto3-batch-1.27.0/mypy_boto3_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:25.958883 mypy-boto3-batch-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:33:06.000000 mypy-boto3-batch-1.27.0/setup.py
```

### Comparing `mypy-boto3-batch-1.26.98/LICENSE` & `mypy-boto3-batch-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.26.98/PKG-INFO` & `mypy-boto3-batch-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.26.98
-Summary: Type annotations for boto3.Batch 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Batch 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-batch"></a>
 
 # mypy-boto3-batch
 
 [![PyPI - mypy-boto3-batch](https://img.shields.io/pypi/v/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-batch?color=blue)](https://pypistats.org/packages/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,25 +376,30 @@
     LaunchTemplateSpecificationTypeDef,
     EphemeralStorageTypeDef,
     FargatePlatformConfigurationTypeDef,
     KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
     ResourceRequirementTypeDef,
+    RuntimePlatformTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    CreateComputeEnvironmentResponseTypeDef,
+    CreateJobQueueResponseTypeDef,
+    CreateSchedulingPolicyResponseTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
     DescribeComputeEnvironmentsRequestRequestTypeDef,
+    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
+    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
     DeviceTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
     EksContainerEnvironmentVariableTypeDef,
@@ -410,40 +415,36 @@
     HostTypeDef,
     JobTimeoutTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
     KeyValuesPairTypeDef,
     TmpfsTypeDef,
+    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    RegisterJobDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
+    SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateComputeEnvironmentResponseTypeDef,
+    UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
     CreateJobQueueRequestRequestTypeDef,
     JobQueueDetailTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
     LogConfigurationTypeDef,
-    CreateComputeEnvironmentResponseTypeDef,
-    CreateJobQueueResponseTypeDef,
-    CreateSchedulingPolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterJobDefinitionResponseTypeDef,
-    SubmitJobResponseTypeDef,
-    UpdateComputeEnvironmentResponseTypeDef,
-    UpdateJobQueueResponseTypeDef,
-    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
-    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
-    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
-    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
     EksContainerOverrideTypeDef,
     EksContainerDetailTypeDef,
     EksContainerTypeDef,
     EksVolumeTypeDef,
     RetryStrategyTypeDef,
```

### Comparing `mypy-boto3-batch-1.26.98/README.md` & `mypy-boto3-batch-1.27.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-batch"></a>
 
 # mypy-boto3-batch
 
 [![PyPI - mypy-boto3-batch](https://img.shields.io/pypi/v/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-batch?color=blue)](https://pypistats.org/packages/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,25 +344,30 @@
     LaunchTemplateSpecificationTypeDef,
     EphemeralStorageTypeDef,
     FargatePlatformConfigurationTypeDef,
     KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
     ResourceRequirementTypeDef,
+    RuntimePlatformTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    CreateComputeEnvironmentResponseTypeDef,
+    CreateJobQueueResponseTypeDef,
+    CreateSchedulingPolicyResponseTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
     DescribeComputeEnvironmentsRequestRequestTypeDef,
+    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
+    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
     DeviceTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
     EksContainerEnvironmentVariableTypeDef,
@@ -378,40 +383,36 @@
     HostTypeDef,
     JobTimeoutTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
     KeyValuesPairTypeDef,
     TmpfsTypeDef,
+    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    RegisterJobDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
+    SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateComputeEnvironmentResponseTypeDef,
+    UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
     CreateJobQueueRequestRequestTypeDef,
     JobQueueDetailTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
     LogConfigurationTypeDef,
-    CreateComputeEnvironmentResponseTypeDef,
-    CreateJobQueueResponseTypeDef,
-    CreateSchedulingPolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterJobDefinitionResponseTypeDef,
-    SubmitJobResponseTypeDef,
-    UpdateComputeEnvironmentResponseTypeDef,
-    UpdateJobQueueResponseTypeDef,
-    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
-    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
-    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
-    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
     EksContainerOverrideTypeDef,
     EksContainerDetailTypeDef,
     EksContainerTypeDef,
     EksVolumeTypeDef,
     RetryStrategyTypeDef,
```

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/__init__.py` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/__init__.pyi` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/__main__.py` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Batch 1.26.98\nVersion:         1.26.98\nBuilder version:"
-        " 7.14.2\nDocs:           "
+        "Type annotations for boto3.Batch 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.98")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/client.py` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/client.pyi` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/literals.py` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -139,14 +140,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -288,14 +290,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -314,16 +317,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -407,15 +413,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -447,21 +455,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/literals.pyi` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -137,14 +138,15 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
+    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -286,14 +288,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -312,16 +315,19 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -405,15 +411,17 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -445,21 +453,25 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/paginator.py` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,106 +46,99 @@
     "DescribeComputeEnvironmentsPaginator",
     "DescribeJobDefinitionsPaginator",
     "DescribeJobQueuesPaginator",
     "ListJobsPaginator",
     "ListSchedulingPoliciesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeComputeEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describecomputeenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeComputeEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describecomputeenvironmentspaginator)
         """
 
-
 class DescribeJobDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobdefinitionspaginator)
         """
 
-
 class DescribeJobQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobqueuespaginator)
     """
 
     def paginate(
-        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobqueuespaginator)
         """
 
-
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listjobspaginator)
     """
 
     def paginate(
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         filters: Sequence[KeyValuesPairTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listjobspaginator)
         """
 
-
 class ListSchedulingPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listschedulingpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchedulingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listschedulingpoliciespaginator)
         """
```

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/paginator.pyi` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,99 +46,106 @@
     "DescribeComputeEnvironmentsPaginator",
     "DescribeJobDefinitionsPaginator",
     "DescribeJobQueuesPaginator",
     "ListJobsPaginator",
     "ListSchedulingPoliciesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeComputeEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describecomputeenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeComputeEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describecomputeenvironmentspaginator)
         """
 
+
 class DescribeJobDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobdefinitionspaginator)
     """
 
     def paginate(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobdefinitionspaginator)
         """
 
+
 class DescribeJobQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobqueuespaginator)
     """
 
     def paginate(
-        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[DescribeJobQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#describejobqueuespaginator)
         """
 
+
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listjobspaginator)
     """
 
     def paginate(
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         filters: Sequence[KeyValuesPairTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listjobspaginator)
         """
 
+
 class ListSchedulingPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listschedulingpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSchedulingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/paginators/#listschedulingpoliciespaginator)
         """
```

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/type_defs.py` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,25 +56,30 @@
     "LaunchTemplateSpecificationTypeDef",
     "EphemeralStorageTypeDef",
     "FargatePlatformConfigurationTypeDef",
     "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "NetworkConfigurationTypeDef",
     "ResourceRequirementTypeDef",
+    "RuntimePlatformTypeDef",
     "SecretTypeDef",
     "UlimitTypeDef",
     "ContainerSummaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateComputeEnvironmentResponseTypeDef",
+    "CreateJobQueueResponseTypeDef",
+    "CreateSchedulingPolicyResponseTypeDef",
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     "DeleteJobQueueRequestRequestTypeDef",
     "DeleteSchedulingPolicyRequestRequestTypeDef",
     "DeregisterJobDefinitionRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
     "DescribeJobDefinitionsRequestRequestTypeDef",
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
     "DescribeJobQueuesRequestRequestTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
     "DeviceTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EksAttemptContainerDetailTypeDef",
     "EksContainerEnvironmentVariableTypeDef",
@@ -90,40 +95,36 @@
     "HostTypeDef",
     "JobTimeoutTypeDef",
     "JobDependencyTypeDef",
     "NodeDetailsTypeDef",
     "NodePropertiesSummaryTypeDef",
     "KeyValuesPairTypeDef",
     "TmpfsTypeDef",
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "ListSchedulingPoliciesRequestRequestTypeDef",
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "RegisterJobDefinitionResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "SubmitJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateComputeEnvironmentResponseTypeDef",
+    "UpdateJobQueueResponseTypeDef",
     "AttemptContainerDetailTypeDef",
     "CreateJobQueueRequestRequestTypeDef",
     "JobQueueDetailTypeDef",
     "UpdateJobQueueRequestRequestTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
     "ContainerOverridesTypeDef",
     "LogConfigurationTypeDef",
-    "CreateComputeEnvironmentResponseTypeDef",
-    "CreateJobQueueResponseTypeDef",
-    "CreateSchedulingPolicyResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RegisterJobDefinitionResponseTypeDef",
-    "SubmitJobResponseTypeDef",
-    "UpdateComputeEnvironmentResponseTypeDef",
-    "UpdateJobQueueResponseTypeDef",
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "EksAttemptDetailTypeDef",
     "EksContainerOverrideTypeDef",
     "EksContainerDetailTypeDef",
     "EksContainerTypeDef",
     "EksVolumeTypeDef",
     "RetryStrategyTypeDef",
@@ -311,14 +312,23 @@
     "ResourceRequirementTypeDef",
     {
         "value": str,
         "type": ResourceTypeType,
     },
 )
 
+RuntimePlatformTypeDef = TypedDict(
+    "RuntimePlatformTypeDef",
+    {
+        "operatingSystemFamily": str,
+        "cpuArchitecture": str,
+    },
+    total=False,
+)
+
 SecretTypeDef = TypedDict(
     "SecretTypeDef",
     {
         "name": str,
         "valueFrom": str,
     },
 )
@@ -337,22 +347,38 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateComputeEnvironmentResponseTypeDef = TypedDict(
+    "CreateComputeEnvironmentResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateJobQueueResponseTypeDef = TypedDict(
+    "CreateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSchedulingPolicyResponseTypeDef = TypedDict(
+    "CreateSchedulingPolicyResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironment": str,
@@ -376,46 +402,65 @@
 DeregisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinition": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "computeEnvironments": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeComputeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
     {
         "computeEnvironments": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    {
+        "jobDefinitions": Sequence[str],
+        "jobDefinitionName": str,
+        "status": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeJobDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeJobDefinitionsRequestRequestTypeDef",
     {
         "jobDefinitions": Sequence[str],
         "maxResults": int,
         "jobDefinitionName": str,
         "status": str,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    {
+        "jobQueues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeJobQueuesRequestRequestTypeDef = TypedDict(
     "DescribeJobQueuesRequestRequestTypeDef",
     {
         "jobQueues": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -679,14 +724,22 @@
 )
 
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
 
+ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "ListSchedulingPoliciesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -702,14 +755,63 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+RegisterJobDefinitionResponseTypeDef = TypedDict(
+    "RegisterJobDefinitionResponseTypeDef",
+    {
+        "jobDefinitionName": str,
+        "jobDefinitionArn": str,
+        "revision": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+SubmitJobResponseTypeDef = TypedDict(
+    "SubmitJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobName": str,
+        "jobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -726,14 +828,32 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateComputeEnvironmentResponseTypeDef = TypedDict(
+    "UpdateComputeEnvironmentResponseTypeDef",
+    {
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateJobQueueResponseTypeDef = TypedDict(
+    "UpdateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttemptContainerDetailTypeDef = TypedDict(
     "AttemptContainerDetailTypeDef",
     {
         "containerInstanceArn": str,
         "taskArn": str,
         "exitCode": int,
         "reason": str,
@@ -905,124 +1025,14 @@
 )
 
 
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
 
-CreateComputeEnvironmentResponseTypeDef = TypedDict(
-    "CreateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobQueueResponseTypeDef = TypedDict(
-    "CreateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchedulingPolicyResponseTypeDef = TypedDict(
-    "CreateSchedulingPolicyResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterJobDefinitionResponseTypeDef = TypedDict(
-    "RegisterJobDefinitionResponseTypeDef",
-    {
-        "jobDefinitionName": str,
-        "jobDefinitionArn": str,
-        "revision": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubmitJobResponseTypeDef = TypedDict(
-    "SubmitJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobName": str,
-        "jobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateComputeEnvironmentResponseTypeDef = TypedDict(
-    "UpdateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobQueueResponseTypeDef = TypedDict(
-    "UpdateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
-    {
-        "computeEnvironments": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
-    {
-        "jobDefinitions": Sequence[str],
-        "jobDefinitionName": str,
-        "status": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
-    {
-        "jobQueues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -1185,15 +1195,15 @@
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "jobQueue": str,
         "arrayJobId": str,
         "multiNodeJobId": str,
         "jobStatus": JobStatusType,
         "filters": Sequence[KeyValuesPairTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
@@ -1222,15 +1232,15 @@
 )
 
 ListSchedulingPoliciesResponseTypeDef = TypedDict(
     "ListSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyListingDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttemptDetailTypeDef = TypedDict(
     "AttemptDetailTypeDef",
     {
         "container": AttemptContainerDetailTypeDef,
@@ -1242,15 +1252,15 @@
 )
 
 DescribeJobQueuesResponseTypeDef = TypedDict(
     "DescribeJobQueuesResponseTypeDef",
     {
         "jobQueues": List[JobQueueDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredComputeEnvironmentDetailTypeDef = TypedDict(
     "_RequiredComputeEnvironmentDetailTypeDef",
     {
         "computeEnvironmentName": str,
@@ -1384,14 +1394,15 @@
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerDetailTypeDef],
         "volumes": List[EksVolumeTypeDef],
         "podName": str,
         "nodeName": str,
+        "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesTypeDef = TypedDict(
     "EksPodPropertiesTypeDef",
     {
@@ -1474,24 +1485,24 @@
 
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobSummaryList": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeComputeEnvironmentsResponseTypeDef = TypedDict(
     "DescribeComputeEnvironmentsResponseTypeDef",
     {
         "computeEnvironments": List[ComputeEnvironmentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NodeOverridesTypeDef = TypedDict(
     "NodeOverridesTypeDef",
     {
         "numNodes": int,
@@ -1526,14 +1537,15 @@
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 ContainerPropertiesTypeDef = TypedDict(
     "ContainerPropertiesTypeDef",
     {
@@ -1554,14 +1566,15 @@
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 EksPropertiesOverrideTypeDef = TypedDict(
     "EksPropertiesOverrideTypeDef",
     {
@@ -1586,15 +1599,15 @@
     total=False,
 )
 
 DescribeSchedulingPoliciesResponseTypeDef = TypedDict(
     "DescribeSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredNodeRangePropertyTypeDef = TypedDict(
     "_RequiredNodeRangePropertyTypeDef",
     {
         "targetNodes": str,
@@ -1769,18 +1782,18 @@
 
 
 DescribeJobDefinitionsResponseTypeDef = TypedDict(
     "DescribeJobDefinitionsResponseTypeDef",
     {
         "jobDefinitions": List[JobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "jobs": List[JobDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch/type_defs.pyi` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,25 +55,30 @@
     "LaunchTemplateSpecificationTypeDef",
     "EphemeralStorageTypeDef",
     "FargatePlatformConfigurationTypeDef",
     "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "NetworkConfigurationTypeDef",
     "ResourceRequirementTypeDef",
+    "RuntimePlatformTypeDef",
     "SecretTypeDef",
     "UlimitTypeDef",
     "ContainerSummaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateComputeEnvironmentResponseTypeDef",
+    "CreateJobQueueResponseTypeDef",
+    "CreateSchedulingPolicyResponseTypeDef",
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     "DeleteJobQueueRequestRequestTypeDef",
     "DeleteSchedulingPolicyRequestRequestTypeDef",
     "DeregisterJobDefinitionRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
     "DescribeJobDefinitionsRequestRequestTypeDef",
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
     "DescribeJobQueuesRequestRequestTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
     "DeviceTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EksAttemptContainerDetailTypeDef",
     "EksContainerEnvironmentVariableTypeDef",
@@ -89,40 +94,36 @@
     "HostTypeDef",
     "JobTimeoutTypeDef",
     "JobDependencyTypeDef",
     "NodeDetailsTypeDef",
     "NodePropertiesSummaryTypeDef",
     "KeyValuesPairTypeDef",
     "TmpfsTypeDef",
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "ListSchedulingPoliciesRequestRequestTypeDef",
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "RegisterJobDefinitionResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "SubmitJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateComputeEnvironmentResponseTypeDef",
+    "UpdateJobQueueResponseTypeDef",
     "AttemptContainerDetailTypeDef",
     "CreateJobQueueRequestRequestTypeDef",
     "JobQueueDetailTypeDef",
     "UpdateJobQueueRequestRequestTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
     "ContainerOverridesTypeDef",
     "LogConfigurationTypeDef",
-    "CreateComputeEnvironmentResponseTypeDef",
-    "CreateJobQueueResponseTypeDef",
-    "CreateSchedulingPolicyResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "RegisterJobDefinitionResponseTypeDef",
-    "SubmitJobResponseTypeDef",
-    "UpdateComputeEnvironmentResponseTypeDef",
-    "UpdateJobQueueResponseTypeDef",
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "EksAttemptDetailTypeDef",
     "EksContainerOverrideTypeDef",
     "EksContainerDetailTypeDef",
     "EksContainerTypeDef",
     "EksVolumeTypeDef",
     "RetryStrategyTypeDef",
@@ -308,14 +309,23 @@
     "ResourceRequirementTypeDef",
     {
         "value": str,
         "type": ResourceTypeType,
     },
 )
 
+RuntimePlatformTypeDef = TypedDict(
+    "RuntimePlatformTypeDef",
+    {
+        "operatingSystemFamily": str,
+        "cpuArchitecture": str,
+    },
+    total=False,
+)
+
 SecretTypeDef = TypedDict(
     "SecretTypeDef",
     {
         "name": str,
         "valueFrom": str,
     },
 )
@@ -334,22 +344,38 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateComputeEnvironmentResponseTypeDef = TypedDict(
+    "CreateComputeEnvironmentResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateJobQueueResponseTypeDef = TypedDict(
+    "CreateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateSchedulingPolicyResponseTypeDef = TypedDict(
+    "CreateSchedulingPolicyResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironment": str,
@@ -373,46 +399,65 @@
 DeregisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinition": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "computeEnvironments": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 DescribeComputeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
     {
         "computeEnvironments": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    {
+        "jobDefinitions": Sequence[str],
+        "jobDefinitionName": str,
+        "status": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeJobDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeJobDefinitionsRequestRequestTypeDef",
     {
         "jobDefinitions": Sequence[str],
         "maxResults": int,
         "jobDefinitionName": str,
         "status": str,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    {
+        "jobQueues": Sequence[str],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 DescribeJobQueuesRequestRequestTypeDef = TypedDict(
     "DescribeJobQueuesRequestRequestTypeDef",
     {
         "jobQueues": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -664,14 +709,22 @@
     },
     total=False,
 )
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
+ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "ListSchedulingPoliciesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -687,14 +740,63 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+RegisterJobDefinitionResponseTypeDef = TypedDict(
+    "RegisterJobDefinitionResponseTypeDef",
+    {
+        "jobDefinitionName": str,
+        "jobDefinitionArn": str,
+        "revision": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+SubmitJobResponseTypeDef = TypedDict(
+    "SubmitJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobName": str,
+        "jobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -711,14 +813,32 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+UpdateComputeEnvironmentResponseTypeDef = TypedDict(
+    "UpdateComputeEnvironmentResponseTypeDef",
+    {
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateJobQueueResponseTypeDef = TypedDict(
+    "UpdateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttemptContainerDetailTypeDef = TypedDict(
     "AttemptContainerDetailTypeDef",
     {
         "containerInstanceArn": str,
         "taskArn": str,
         "exitCode": int,
         "reason": str,
@@ -880,124 +1000,14 @@
     },
     total=False,
 )
 
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
-CreateComputeEnvironmentResponseTypeDef = TypedDict(
-    "CreateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateJobQueueResponseTypeDef = TypedDict(
-    "CreateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateSchedulingPolicyResponseTypeDef = TypedDict(
-    "CreateSchedulingPolicyResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RegisterJobDefinitionResponseTypeDef = TypedDict(
-    "RegisterJobDefinitionResponseTypeDef",
-    {
-        "jobDefinitionName": str,
-        "jobDefinitionArn": str,
-        "revision": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SubmitJobResponseTypeDef = TypedDict(
-    "SubmitJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobName": str,
-        "jobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateComputeEnvironmentResponseTypeDef = TypedDict(
-    "UpdateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateJobQueueResponseTypeDef = TypedDict(
-    "UpdateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
-    {
-        "computeEnvironments": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
-    {
-        "jobDefinitions": Sequence[str],
-        "jobDefinitionName": str,
-        "status": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
-    {
-        "jobQueues": Sequence[str],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -1152,15 +1162,15 @@
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "jobQueue": str,
         "arrayJobId": str,
         "multiNodeJobId": str,
         "jobStatus": JobStatusType,
         "filters": Sequence[KeyValuesPairTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
@@ -1189,15 +1199,15 @@
 )
 
 ListSchedulingPoliciesResponseTypeDef = TypedDict(
     "ListSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyListingDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttemptDetailTypeDef = TypedDict(
     "AttemptDetailTypeDef",
     {
         "container": AttemptContainerDetailTypeDef,
@@ -1209,15 +1219,15 @@
 )
 
 DescribeJobQueuesResponseTypeDef = TypedDict(
     "DescribeJobQueuesResponseTypeDef",
     {
         "jobQueues": List[JobQueueDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredComputeEnvironmentDetailTypeDef = TypedDict(
     "_RequiredComputeEnvironmentDetailTypeDef",
     {
         "computeEnvironmentName": str,
@@ -1343,14 +1353,15 @@
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerDetailTypeDef],
         "volumes": List[EksVolumeTypeDef],
         "podName": str,
         "nodeName": str,
+        "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesTypeDef = TypedDict(
     "EksPodPropertiesTypeDef",
     {
@@ -1427,24 +1438,24 @@
     pass
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobSummaryList": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeComputeEnvironmentsResponseTypeDef = TypedDict(
     "DescribeComputeEnvironmentsResponseTypeDef",
     {
         "computeEnvironments": List[ComputeEnvironmentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 NodeOverridesTypeDef = TypedDict(
     "NodeOverridesTypeDef",
     {
         "numNodes": int,
@@ -1479,14 +1490,15 @@
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 ContainerPropertiesTypeDef = TypedDict(
     "ContainerPropertiesTypeDef",
     {
@@ -1507,14 +1519,15 @@
         "resourceRequirements": List[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
     },
     total=False,
 )
 
 EksPropertiesOverrideTypeDef = TypedDict(
     "EksPropertiesOverrideTypeDef",
     {
@@ -1539,15 +1552,15 @@
     total=False,
 )
 
 DescribeSchedulingPoliciesResponseTypeDef = TypedDict(
     "DescribeSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredNodeRangePropertyTypeDef = TypedDict(
     "_RequiredNodeRangePropertyTypeDef",
     {
         "targetNodes": str,
@@ -1712,18 +1725,18 @@
     pass
 
 DescribeJobDefinitionsResponseTypeDef = TypedDict(
     "DescribeJobDefinitionsResponseTypeDef",
     {
         "jobDefinitions": List[JobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "jobs": List[JobDetailTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch.egg-info/PKG-INFO` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-batch
-Version: 1.26.98
-Summary: Type annotations for boto3.Batch 1.26.98 service generated with mypy-boto3-builder 7.14.2
+Version: 1.27.0
+Summary: Type annotations for boto3.Batch 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-batch"></a>
 
 # mypy-boto3-batch
 
 [![PyPI - mypy-boto3-batch](https://img.shields.io/pypi/v/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-batch.svg?color=blue)](https://pypi.org/project/mypy-boto3-batch)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-batch?color=blue)](https://pypistats.org/packages/mypy-boto3-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Batch 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
+[boto3.Batch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-batch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,25 +376,30 @@
     LaunchTemplateSpecificationTypeDef,
     EphemeralStorageTypeDef,
     FargatePlatformConfigurationTypeDef,
     KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
     ResourceRequirementTypeDef,
+    RuntimePlatformTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    CreateComputeEnvironmentResponseTypeDef,
+    CreateJobQueueResponseTypeDef,
+    CreateSchedulingPolicyResponseTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
     DescribeComputeEnvironmentsRequestRequestTypeDef,
+    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
+    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
     DeviceTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
     EksContainerEnvironmentVariableTypeDef,
@@ -410,40 +415,36 @@
     HostTypeDef,
     JobTimeoutTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
     KeyValuesPairTypeDef,
     TmpfsTypeDef,
+    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    RegisterJobDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
+    SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateComputeEnvironmentResponseTypeDef,
+    UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
     CreateJobQueueRequestRequestTypeDef,
     JobQueueDetailTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
     LogConfigurationTypeDef,
-    CreateComputeEnvironmentResponseTypeDef,
-    CreateJobQueueResponseTypeDef,
-    CreateSchedulingPolicyResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RegisterJobDefinitionResponseTypeDef,
-    SubmitJobResponseTypeDef,
-    UpdateComputeEnvironmentResponseTypeDef,
-    UpdateJobQueueResponseTypeDef,
-    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
-    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
-    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
-    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
     EksContainerOverrideTypeDef,
     EksContainerDetailTypeDef,
     EksContainerTypeDef,
     EksVolumeTypeDef,
     RetryStrategyTypeDef,
```

### Comparing `mypy-boto3-batch-1.26.98/mypy_boto3_batch.egg-info/SOURCES.txt` & `mypy-boto3-batch-1.27.0/mypy_boto3_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-batch-1.26.98/setup.py` & `mypy-boto3-batch-1.27.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-batch",
-    version="1.26.98",
+    version="1.27.0",
     packages=["mypy_boto3_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Batch 1.26.98 service generated with mypy-boto3-builder 7.14.2"
+        "Type annotations for boto3.Batch 1.27.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

