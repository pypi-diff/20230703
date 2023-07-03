# Comparing `tmp/mypy-boto3-comprehendmedical-1.26.150.tar.gz` & `tmp/mypy-boto3-comprehendmedical-1.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehendmedical-1.26.150.tar", last modified: Thu Jun  8 19:32:29 2023, max compression
+gzip compressed data, was "mypy-boto3-comprehendmedical-1.27.0.tar", last modified: Mon Jul  3 19:50:34 2023, max compression
```

## Comparing `mypy-boto3-comprehendmedical-1.26.150.tar` & `mypy-boto3-comprehendmedical-1.27.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21547 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24890 2023-06-08 19:32:10.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.727038 mypy-boto3-comprehendmedical-1.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:43.000000 mypy-boto3-comprehendmedical-1.27.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-07-03 19:50:34.727038 mypy-boto3-comprehendmedical-1.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-03 19:34:43.000000 mypy-boto3-comprehendmedical-1.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.727038 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 19:34:43.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 19:34:43.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-03 19:34:43.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-07-03 19:34:44.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21547 2023-07-03 19:34:44.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-03 19:34:44.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-07-03 19:34:44.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:43.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24942 2023-07-03 19:34:45.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-07-03 19:34:45.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:43.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:34.727038 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-07-03 19:50:34.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 19:50:34.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:34.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:34.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:34.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:34.000000 mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:34.727038 mypy-boto3-comprehendmedical-1.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-03 19:34:43.000000 mypy-boto3-comprehendmedical-1.27.0/setup.py
```

### Comparing `mypy-boto3-comprehendmedical-1.26.150/LICENSE` & `mypy-boto3-comprehendmedical-1.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.26.150/PKG-INFO` & `mypy-boto3-comprehendmedical-1.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.26.150
-Summary: Type annotations for boto3.ComprehendMedical 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.ComprehendMedical 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehendmedical?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -323,59 +323,59 @@
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
     ComprehendMedicalAsyncJobFilterTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
+    ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
+    StartEntitiesDetectionV2JobResponseTypeDef,
+    StartICD10CMInferenceJobResponseTypeDef,
+    StartPHIDetectionJobResponseTypeDef,
+    StartRxNormInferenceJobResponseTypeDef,
+    StartSNOMEDCTInferenceJobResponseTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
+    StopEntitiesDetectionV2JobResponseTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
+    StopICD10CMInferenceJobResponseTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
+    StopPHIDetectionJobResponseTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
+    StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
+    StopSNOMEDCTInferenceJobResponseTypeDef,
     AttributeTypeDef,
     ListEntitiesDetectionV2JobsRequestRequestTypeDef,
     ListICD10CMInferenceJobsRequestRequestTypeDef,
     ListPHIDetectionJobsRequestRequestTypeDef,
     ListRxNormInferenceJobsRequestRequestTypeDef,
     ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
-    StartEntitiesDetectionV2JobResponseTypeDef,
-    StartICD10CMInferenceJobResponseTypeDef,
-    StartPHIDetectionJobResponseTypeDef,
-    StartRxNormInferenceJobResponseTypeDef,
-    StartSNOMEDCTInferenceJobResponseTypeDef,
-    StopEntitiesDetectionV2JobResponseTypeDef,
-    StopICD10CMInferenceJobResponseTypeDef,
-    StopPHIDetectionJobResponseTypeDef,
-    StopRxNormInferenceJobResponseTypeDef,
-    StopSNOMEDCTInferenceJobResponseTypeDef,
     ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
```

### Comparing `mypy-boto3-comprehendmedical-1.26.150/README.md` & `mypy-boto3-comprehendmedical-1.27.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehendmedical?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -291,59 +291,59 @@
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
     ComprehendMedicalAsyncJobFilterTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
+    ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
+    StartEntitiesDetectionV2JobResponseTypeDef,
+    StartICD10CMInferenceJobResponseTypeDef,
+    StartPHIDetectionJobResponseTypeDef,
+    StartRxNormInferenceJobResponseTypeDef,
+    StartSNOMEDCTInferenceJobResponseTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
+    StopEntitiesDetectionV2JobResponseTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
+    StopICD10CMInferenceJobResponseTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
+    StopPHIDetectionJobResponseTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
+    StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
+    StopSNOMEDCTInferenceJobResponseTypeDef,
     AttributeTypeDef,
     ListEntitiesDetectionV2JobsRequestRequestTypeDef,
     ListICD10CMInferenceJobsRequestRequestTypeDef,
     ListPHIDetectionJobsRequestRequestTypeDef,
     ListRxNormInferenceJobsRequestRequestTypeDef,
     ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
-    StartEntitiesDetectionV2JobResponseTypeDef,
-    StartICD10CMInferenceJobResponseTypeDef,
-    StartPHIDetectionJobResponseTypeDef,
-    StartRxNormInferenceJobResponseTypeDef,
-    StartSNOMEDCTInferenceJobResponseTypeDef,
-    StopEntitiesDetectionV2JobResponseTypeDef,
-    StopICD10CMInferenceJobResponseTypeDef,
-    StopPHIDetectionJobResponseTypeDef,
-    StopRxNormInferenceJobResponseTypeDef,
-    StopSNOMEDCTInferenceJobResponseTypeDef,
     ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
```

### Comparing `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/__main__.py` & `mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComprehendMedical 1.26.150\nVersion:         1.26.150\nBuilder"
+        "Type annotations for boto3.ComprehendMedical 1.27.0\nVersion:         1.27.0\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.150")
+    print("1.27.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/client.py` & `mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/client.pyi` & `mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/literals.py` & `mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
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
@@ -253,14 +254,15 @@
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
@@ -525,14 +527,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/literals.pyi` & `mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
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
@@ -251,14 +252,15 @@
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
@@ -523,14 +525,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
+    "verifiedpermissions",
     "voice-id",
     "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
```

### Comparing `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/type_defs.py` & `mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,59 +48,59 @@
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
     "ComprehendMedicalAsyncJobFilterTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
     "DescribeSNOMEDCTInferenceJobRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "DetectEntitiesV2RequestRequestTypeDef",
     "DetectPHIRequestRequestTypeDef",
     "ICD10CMTraitTypeDef",
     "ICD10CMConceptTypeDef",
     "InferICD10CMRequestRequestTypeDef",
     "InferRxNormRequestRequestTypeDef",
     "InferSNOMEDCTRequestRequestTypeDef",
     "SNOMEDCTDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "RxNormTraitTypeDef",
     "RxNormConceptTypeDef",
     "SNOMEDCTConceptTypeDef",
     "SNOMEDCTTraitTypeDef",
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    "StartICD10CMInferenceJobResponseTypeDef",
+    "StartPHIDetectionJobResponseTypeDef",
+    "StartRxNormInferenceJobResponseTypeDef",
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
+    "StopEntitiesDetectionV2JobResponseTypeDef",
     "StopICD10CMInferenceJobRequestRequestTypeDef",
+    "StopICD10CMInferenceJobResponseTypeDef",
     "StopPHIDetectionJobRequestRequestTypeDef",
+    "StopPHIDetectionJobResponseTypeDef",
     "StopRxNormInferenceJobRequestRequestTypeDef",
+    "StopRxNormInferenceJobResponseTypeDef",
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "AttributeTypeDef",
     "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
     "ListICD10CMInferenceJobsRequestRequestTypeDef",
     "ListPHIDetectionJobsRequestRequestTypeDef",
     "ListRxNormInferenceJobsRequestRequestTypeDef",
     "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    "StartICD10CMInferenceJobResponseTypeDef",
-    "StartPHIDetectionJobResponseTypeDef",
-    "StartRxNormInferenceJobResponseTypeDef",
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
-    "StopEntitiesDetectionV2JobResponseTypeDef",
-    "StopICD10CMInferenceJobResponseTypeDef",
-    "StopPHIDetectionJobResponseTypeDef",
-    "StopRxNormInferenceJobResponseTypeDef",
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
@@ -192,25 +192,14 @@
 DescribeEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 DescribeICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -302,14 +291,25 @@
         "Edition": str,
         "Language": str,
         "VersionDate": str,
     },
     total=False,
 )
 
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
 RxNormTraitTypeDef = TypedDict(
     "RxNormTraitTypeDef",
     {
         "Name": RxNormTraitNameType,
         "Score": float,
     },
     total=False,
@@ -340,49 +340,129 @@
     {
         "Name": SNOMEDCTTraitNameType,
         "Score": float,
     },
     total=False,
 )
 
+StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StartICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartPHIDetectionJobResponseTypeDef = TypedDict(
+    "StartPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StartRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "StopICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StopICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopPHIDetectionJobRequestRequestTypeDef = TypedDict(
     "StopPHIDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopPHIDetectionJobResponseTypeDef = TypedDict(
+    "StopPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopRxNormInferenceJobRequestRequestTypeDef = TypedDict(
     "StopRxNormInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StopRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopSNOMEDCTInferenceJobRequestRequestTypeDef = TypedDict(
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Type": EntitySubTypeType,
         "Score": float,
         "RelationshipScore": float,
         "RelationshipType": RelationshipTypeType,
@@ -598,94 +678,14 @@
 class StartSNOMEDCTInferenceJobRequestRequestTypeDef(
     _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef,
     _OptionalStartSNOMEDCTInferenceJobRequestRequestTypeDef,
 ):
     pass
 
 
-StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StartICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartPHIDetectionJobResponseTypeDef = TypedDict(
-    "StartPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StartRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StopICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopPHIDetectionJobResponseTypeDef = TypedDict(
-    "StopPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StopRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ICD10CMAttributeTypeDef = TypedDict(
     "ICD10CMAttributeTypeDef",
     {
         "Type": ICD10CMAttributeTypeType,
         "Score": float,
         "RelationshipScore": float,
         "Id": int,
@@ -757,92 +757,92 @@
     total=False,
 )
 
 DescribeEntitiesDetectionV2JobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeICD10CMInferenceJobResponseTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePHIDetectionJobResponseTypeDef = TypedDict(
     "DescribePHIDetectionJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRxNormInferenceJobResponseTypeDef = TypedDict(
     "DescribeRxNormInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitiesDetectionV2JobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListICD10CMInferenceJobsResponseTypeDef = TypedDict(
     "ListICD10CMInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPHIDetectionJobsResponseTypeDef = TypedDict(
     "ListPHIDetectionJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRxNormInferenceJobsResponseTypeDef = TypedDict(
     "ListRxNormInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSNOMEDCTInferenceJobsResponseTypeDef = TypedDict(
     "ListSNOMEDCTInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ICD10CMEntityTypeDef = TypedDict(
     "ICD10CMEntityTypeDef",
     {
         "Id": int,
@@ -895,64 +895,64 @@
 
 DetectPHIResponseTypeDef = TypedDict(
     "DetectPHIResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectEntitiesResponseTypeDef = TypedDict(
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectEntitiesV2ResponseTypeDef = TypedDict(
     "DetectEntitiesV2ResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InferICD10CMResponseTypeDef = TypedDict(
     "InferICD10CMResponseTypeDef",
     {
         "Entities": List[ICD10CMEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InferRxNormResponseTypeDef = TypedDict(
     "InferRxNormResponseTypeDef",
     {
         "Entities": List[RxNormEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InferSNOMEDCTResponseTypeDef = TypedDict(
     "InferSNOMEDCTResponseTypeDef",
     {
         "Entities": List[SNOMEDCTEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
         "SNOMEDCTDetails": SNOMEDCTDetailsTypeDef,
         "Characters": CharactersTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/type_defs.pyi` & `mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -47,59 +47,59 @@
 __all__ = (
     "TraitTypeDef",
     "CharactersTypeDef",
     "ComprehendMedicalAsyncJobFilterTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     "DescribePHIDetectionJobRequestRequestTypeDef",
     "DescribeRxNormInferenceJobRequestRequestTypeDef",
     "DescribeSNOMEDCTInferenceJobRequestRequestTypeDef",
     "DetectEntitiesRequestRequestTypeDef",
     "DetectEntitiesV2RequestRequestTypeDef",
     "DetectPHIRequestRequestTypeDef",
     "ICD10CMTraitTypeDef",
     "ICD10CMConceptTypeDef",
     "InferICD10CMRequestRequestTypeDef",
     "InferRxNormRequestRequestTypeDef",
     "InferSNOMEDCTRequestRequestTypeDef",
     "SNOMEDCTDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "RxNormTraitTypeDef",
     "RxNormConceptTypeDef",
     "SNOMEDCTConceptTypeDef",
     "SNOMEDCTTraitTypeDef",
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    "StartICD10CMInferenceJobResponseTypeDef",
+    "StartPHIDetectionJobResponseTypeDef",
+    "StartRxNormInferenceJobResponseTypeDef",
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
+    "StopEntitiesDetectionV2JobResponseTypeDef",
     "StopICD10CMInferenceJobRequestRequestTypeDef",
+    "StopICD10CMInferenceJobResponseTypeDef",
     "StopPHIDetectionJobRequestRequestTypeDef",
+    "StopPHIDetectionJobResponseTypeDef",
     "StopRxNormInferenceJobRequestRequestTypeDef",
+    "StopRxNormInferenceJobResponseTypeDef",
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "AttributeTypeDef",
     "ListEntitiesDetectionV2JobsRequestRequestTypeDef",
     "ListICD10CMInferenceJobsRequestRequestTypeDef",
     "ListPHIDetectionJobsRequestRequestTypeDef",
     "ListRxNormInferenceJobsRequestRequestTypeDef",
     "ListSNOMEDCTInferenceJobsRequestRequestTypeDef",
     "ComprehendMedicalAsyncJobPropertiesTypeDef",
     "StartEntitiesDetectionV2JobRequestRequestTypeDef",
     "StartICD10CMInferenceJobRequestRequestTypeDef",
     "StartPHIDetectionJobRequestRequestTypeDef",
     "StartRxNormInferenceJobRequestRequestTypeDef",
     "StartSNOMEDCTInferenceJobRequestRequestTypeDef",
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    "StartICD10CMInferenceJobResponseTypeDef",
-    "StartPHIDetectionJobResponseTypeDef",
-    "StartRxNormInferenceJobResponseTypeDef",
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
-    "StopEntitiesDetectionV2JobResponseTypeDef",
-    "StopICD10CMInferenceJobResponseTypeDef",
-    "StopPHIDetectionJobResponseTypeDef",
-    "StopRxNormInferenceJobResponseTypeDef",
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
     "ICD10CMAttributeTypeDef",
     "RxNormAttributeTypeDef",
     "SNOMEDCTAttributeTypeDef",
     "EntityTypeDef",
     "UnmappedAttributeTypeDef",
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     "DescribeICD10CMInferenceJobResponseTypeDef",
@@ -187,25 +187,14 @@
 DescribeEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 DescribeICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -297,14 +286,25 @@
         "Edition": str,
         "Language": str,
         "VersionDate": str,
     },
     total=False,
 )
 
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
 RxNormTraitTypeDef = TypedDict(
     "RxNormTraitTypeDef",
     {
         "Name": RxNormTraitNameType,
         "Score": float,
     },
     total=False,
@@ -335,49 +335,129 @@
     {
         "Name": SNOMEDCTTraitNameType,
         "Score": float,
     },
     total=False,
 )
 
+StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StartEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StartICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartPHIDetectionJobResponseTypeDef = TypedDict(
+    "StartPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StartRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StartSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopEntitiesDetectionV2JobRequestRequestTypeDef = TypedDict(
     "StopEntitiesDetectionV2JobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
+    "StopEntitiesDetectionV2JobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopICD10CMInferenceJobRequestRequestTypeDef = TypedDict(
     "StopICD10CMInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopICD10CMInferenceJobResponseTypeDef = TypedDict(
+    "StopICD10CMInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopPHIDetectionJobRequestRequestTypeDef = TypedDict(
     "StopPHIDetectionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopPHIDetectionJobResponseTypeDef = TypedDict(
+    "StopPHIDetectionJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopRxNormInferenceJobRequestRequestTypeDef = TypedDict(
     "StopRxNormInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopRxNormInferenceJobResponseTypeDef = TypedDict(
+    "StopRxNormInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 StopSNOMEDCTInferenceJobRequestRequestTypeDef = TypedDict(
     "StopSNOMEDCTInferenceJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
+    "StopSNOMEDCTInferenceJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "Type": EntitySubTypeType,
         "Score": float,
         "RelationshipScore": float,
         "RelationshipType": RelationshipTypeType,
@@ -583,94 +663,14 @@
 
 class StartSNOMEDCTInferenceJobRequestRequestTypeDef(
     _RequiredStartSNOMEDCTInferenceJobRequestRequestTypeDef,
     _OptionalStartSNOMEDCTInferenceJobRequestRequestTypeDef,
 ):
     pass
 
-StartEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StartEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StartICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartPHIDetectionJobResponseTypeDef = TypedDict(
-    "StartPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StartRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StartSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopEntitiesDetectionV2JobResponseTypeDef = TypedDict(
-    "StopEntitiesDetectionV2JobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopICD10CMInferenceJobResponseTypeDef = TypedDict(
-    "StopICD10CMInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopPHIDetectionJobResponseTypeDef = TypedDict(
-    "StopPHIDetectionJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopRxNormInferenceJobResponseTypeDef = TypedDict(
-    "StopRxNormInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StopSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
-    "StopSNOMEDCTInferenceJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ICD10CMAttributeTypeDef = TypedDict(
     "ICD10CMAttributeTypeDef",
     {
         "Type": ICD10CMAttributeTypeType,
         "Score": float,
         "RelationshipScore": float,
         "Id": int,
@@ -742,92 +742,92 @@
     total=False,
 )
 
 DescribeEntitiesDetectionV2JobResponseTypeDef = TypedDict(
     "DescribeEntitiesDetectionV2JobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeICD10CMInferenceJobResponseTypeDef = TypedDict(
     "DescribeICD10CMInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribePHIDetectionJobResponseTypeDef = TypedDict(
     "DescribePHIDetectionJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeRxNormInferenceJobResponseTypeDef = TypedDict(
     "DescribeRxNormInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeSNOMEDCTInferenceJobResponseTypeDef = TypedDict(
     "DescribeSNOMEDCTInferenceJobResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobProperties": ComprehendMedicalAsyncJobPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEntitiesDetectionV2JobsResponseTypeDef = TypedDict(
     "ListEntitiesDetectionV2JobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListICD10CMInferenceJobsResponseTypeDef = TypedDict(
     "ListICD10CMInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPHIDetectionJobsResponseTypeDef = TypedDict(
     "ListPHIDetectionJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRxNormInferenceJobsResponseTypeDef = TypedDict(
     "ListRxNormInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSNOMEDCTInferenceJobsResponseTypeDef = TypedDict(
     "ListSNOMEDCTInferenceJobsResponseTypeDef",
     {
         "ComprehendMedicalAsyncJobPropertiesList": List[ComprehendMedicalAsyncJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ICD10CMEntityTypeDef = TypedDict(
     "ICD10CMEntityTypeDef",
     {
         "Id": int,
@@ -880,64 +880,64 @@
 
 DetectPHIResponseTypeDef = TypedDict(
     "DetectPHIResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectEntitiesResponseTypeDef = TypedDict(
     "DetectEntitiesResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DetectEntitiesV2ResponseTypeDef = TypedDict(
     "DetectEntitiesV2ResponseTypeDef",
     {
         "Entities": List[EntityTypeDef],
         "UnmappedAttributes": List[UnmappedAttributeTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InferICD10CMResponseTypeDef = TypedDict(
     "InferICD10CMResponseTypeDef",
     {
         "Entities": List[ICD10CMEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InferRxNormResponseTypeDef = TypedDict(
     "InferRxNormResponseTypeDef",
     {
         "Entities": List[RxNormEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InferSNOMEDCTResponseTypeDef = TypedDict(
     "InferSNOMEDCTResponseTypeDef",
     {
         "Entities": List[SNOMEDCTEntityTypeDef],
         "PaginationToken": str,
         "ModelVersion": str,
         "SNOMEDCTDetails": SNOMEDCTDetailsTypeDef,
         "Characters": CharactersTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/PKG-INFO` & `mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.26.150
-Summary: Type annotations for boto3.ComprehendMedical 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.27.0
+Summary: Type annotations for boto3.ComprehendMedical 1.27.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehendmedical?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -323,59 +323,59 @@
 from mypy_boto3_comprehendmedical.type_defs import (
     TraitTypeDef,
     CharactersTypeDef,
     ComprehendMedicalAsyncJobFilterTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
     DescribeEntitiesDetectionV2JobRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     DescribeICD10CMInferenceJobRequestRequestTypeDef,
     DescribePHIDetectionJobRequestRequestTypeDef,
     DescribeRxNormInferenceJobRequestRequestTypeDef,
     DescribeSNOMEDCTInferenceJobRequestRequestTypeDef,
     DetectEntitiesRequestRequestTypeDef,
     DetectEntitiesV2RequestRequestTypeDef,
     DetectPHIRequestRequestTypeDef,
     ICD10CMTraitTypeDef,
     ICD10CMConceptTypeDef,
     InferICD10CMRequestRequestTypeDef,
     InferRxNormRequestRequestTypeDef,
     InferSNOMEDCTRequestRequestTypeDef,
     SNOMEDCTDetailsTypeDef,
+    ResponseMetadataTypeDef,
     RxNormTraitTypeDef,
     RxNormConceptTypeDef,
     SNOMEDCTConceptTypeDef,
     SNOMEDCTTraitTypeDef,
+    StartEntitiesDetectionV2JobResponseTypeDef,
+    StartICD10CMInferenceJobResponseTypeDef,
+    StartPHIDetectionJobResponseTypeDef,
+    StartRxNormInferenceJobResponseTypeDef,
+    StartSNOMEDCTInferenceJobResponseTypeDef,
     StopEntitiesDetectionV2JobRequestRequestTypeDef,
+    StopEntitiesDetectionV2JobResponseTypeDef,
     StopICD10CMInferenceJobRequestRequestTypeDef,
+    StopICD10CMInferenceJobResponseTypeDef,
     StopPHIDetectionJobRequestRequestTypeDef,
+    StopPHIDetectionJobResponseTypeDef,
     StopRxNormInferenceJobRequestRequestTypeDef,
+    StopRxNormInferenceJobResponseTypeDef,
     StopSNOMEDCTInferenceJobRequestRequestTypeDef,
+    StopSNOMEDCTInferenceJobResponseTypeDef,
     AttributeTypeDef,
     ListEntitiesDetectionV2JobsRequestRequestTypeDef,
     ListICD10CMInferenceJobsRequestRequestTypeDef,
     ListPHIDetectionJobsRequestRequestTypeDef,
     ListRxNormInferenceJobsRequestRequestTypeDef,
     ListSNOMEDCTInferenceJobsRequestRequestTypeDef,
     ComprehendMedicalAsyncJobPropertiesTypeDef,
     StartEntitiesDetectionV2JobRequestRequestTypeDef,
     StartICD10CMInferenceJobRequestRequestTypeDef,
     StartPHIDetectionJobRequestRequestTypeDef,
     StartRxNormInferenceJobRequestRequestTypeDef,
     StartSNOMEDCTInferenceJobRequestRequestTypeDef,
-    StartEntitiesDetectionV2JobResponseTypeDef,
-    StartICD10CMInferenceJobResponseTypeDef,
-    StartPHIDetectionJobResponseTypeDef,
-    StartRxNormInferenceJobResponseTypeDef,
-    StartSNOMEDCTInferenceJobResponseTypeDef,
-    StopEntitiesDetectionV2JobResponseTypeDef,
-    StopICD10CMInferenceJobResponseTypeDef,
-    StopPHIDetectionJobResponseTypeDef,
-    StopRxNormInferenceJobResponseTypeDef,
-    StopSNOMEDCTInferenceJobResponseTypeDef,
     ICD10CMAttributeTypeDef,
     RxNormAttributeTypeDef,
     SNOMEDCTAttributeTypeDef,
     EntityTypeDef,
     UnmappedAttributeTypeDef,
     DescribeEntitiesDetectionV2JobResponseTypeDef,
     DescribeICD10CMInferenceJobResponseTypeDef,
```

### Comparing `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt` & `mypy-boto3-comprehendmedical-1.27.0/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.26.150/setup.py` & `mypy-boto3-comprehendmedical-1.27.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehendmedical",
-    version="1.26.150",
+    version="1.27.0",
     packages=["mypy_boto3_comprehendmedical"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComprehendMedical 1.26.150 service generated with"
+        "Type annotations for boto3.ComprehendMedical 1.27.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

