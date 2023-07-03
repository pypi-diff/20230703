# Comparing `tmp/pasqal-cloud-0.3.1.tar.gz` & `tmp/pasqal-cloud-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.3.1.tar", last modified: Fri Jun 30 12:39:33 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.3.2.tar", last modified: Mon Jul  3 13:26:26 2023, max compression
```

## Comparing `pasqal-cloud-0.3.1.tar` & `pasqal-cloud-0.3.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-30 12:39:33.000000 pasqal-cloud-0.3.1/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.632677 pasqal-cloud-0.3.1/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:33.636677 pasqal-cloud-0.3.1/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-30 12:39:19.000000 pasqal-cloud-0.3.1/tests/test_project_renaming_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.409693 pasqal-cloud-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-03 13:26:26.409693 pasqal-cloud-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.401692 pasqal-cloud-0.3.2/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.401692 pasqal-cloud-0.3.2/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.401692 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 13:26:26.000000 pasqal-cloud-0.3.2/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.405692 pasqal-cloud-0.3.2/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 13:26:26.413693 pasqal-cloud-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.409693 pasqal-cloud-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:26.409693 pasqal-cloud-0.3.2/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-03 13:26:13.000000 pasqal-cloud-0.3.2/tests/test_project_renaming_compatibility.py
```

### Comparing `pasqal-cloud-0.3.1/LICENSE` & `pasqal-cloud-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/PKG-INFO` & `pasqal-cloud-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.3.1
+Version: 0.3.2
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -40,20 +40,26 @@
 
 To run the tutorials or the test suite locally, run the following to install the development requirements:
 
 ```bash
 pip install -e .[dev]
 ```
 
+We use pre-commit hooks to enforce some code linting, you can install pre-commit with Python pip:
+```bash
+python3 -m pip install pre-commit
+pre-commit install
+```
+
 ## Basic usage
 
 The package main component is a python object called `SDK` which can be used to create a `Batch` and send it automatically
 to Pasqal APIs using an API token generated in the [user portal](https://portal.pasqal.cloud).
 
-A `Batch` is a group of jobs with the same sequence that will run on the same QPU. For each job of a given batch you must set a value for each variable, if any, defined in your sequence.  
+A `Batch` is a group of jobs with the same sequence that will run on the same QPU. For each job of a given batch you must set a value for each variable, if any, defined in your sequence.
 The batch sequence can be generated using [Pulser](https://github.com/pasqal-io/Pulser). See their [documentation](https://pulser.readthedocs.io/en/stable/),
 for more information on how to install the library and create your own sequence.
 
 Once you have created your sequence, you should serialize it as follows:
 
 ```python
 # sequence should be a pulser Sequence object
```

### Comparing `pasqal-cloud-0.3.1/README.md` & `pasqal-cloud-0.3.2/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pasqal-cloud
+Version: 0.3.2
+Summary: Software development kit for Pasqal cloud platform.
+Home-page: https://github.com/pasqal-io/pasqal-cloud
+Maintainer: Pasqal Cloud Services
+Maintainer-email: pcs@pasqal.io
+License: Apache 2.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
 
 To install the latest release of the `pasqal-cloud` (formerly pasqal-sdk), have Python 3.8.0 or higher installed, then use pip:
@@ -25,20 +40,26 @@
 
 To run the tutorials or the test suite locally, run the following to install the development requirements:
 
 ```bash
 pip install -e .[dev]
 ```
 
+We use pre-commit hooks to enforce some code linting, you can install pre-commit with Python pip:
+```bash
+python3 -m pip install pre-commit
+pre-commit install
+```
+
 ## Basic usage
 
 The package main component is a python object called `SDK` which can be used to create a `Batch` and send it automatically
 to Pasqal APIs using an API token generated in the [user portal](https://portal.pasqal.cloud).
 
-A `Batch` is a group of jobs with the same sequence that will run on the same QPU. For each job of a given batch you must set a value for each variable, if any, defined in your sequence.  
+A `Batch` is a group of jobs with the same sequence that will run on the same QPU. For each job of a given batch you must set a value for each variable, if any, defined in your sequence.
 The batch sequence can be generated using [Pulser](https://github.com/pasqal-io/Pulser). See their [documentation](https://pulser.readthedocs.io/en/stable/),
 for more information on how to install the library and create your own sequence.
 
 Once you have created your sequence, you should serialize it as follows:
 
 ```python
 # sequence should be a pulser Sequence object
```

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/__init__.py` & `pasqal-cloud-0.3.2/pasqal_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/_version.py` & `pasqal-cloud-0.3.2/pasqal_cloud/_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
```

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/authentication.py` & `pasqal-cloud-0.3.2/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/batch.py` & `pasqal-cloud-0.3.2/pasqal_cloud/batch.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/client.py` & `pasqal-cloud-0.3.2/pasqal_cloud/client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.3.2/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.3.2/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/errors.py` & `pasqal-cloud-0.3.2/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/job.py` & `pasqal-cloud-0.3.2/pasqal_cloud/job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.3.2/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.3.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pasqal-cloud
-Version: 0.3.1
-Summary: Software development kit for Pasqal cloud platform.
-Home-page: https://github.com/pasqal-io/pasqal-cloud
-Maintainer: Pasqal Cloud Services
-Maintainer-email: pcs@pasqal.io
-License: Apache 2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
 
 To install the latest release of the `pasqal-cloud` (formerly pasqal-sdk), have Python 3.8.0 or higher installed, then use pip:
@@ -40,20 +25,26 @@
 
 To run the tutorials or the test suite locally, run the following to install the development requirements:
 
 ```bash
 pip install -e .[dev]
 ```
 
+We use pre-commit hooks to enforce some code linting, you can install pre-commit with Python pip:
+```bash
+python3 -m pip install pre-commit
+pre-commit install
+```
+
 ## Basic usage
 
 The package main component is a python object called `SDK` which can be used to create a `Batch` and send it automatically
 to Pasqal APIs using an API token generated in the [user portal](https://portal.pasqal.cloud).
 
-A `Batch` is a group of jobs with the same sequence that will run on the same QPU. For each job of a given batch you must set a value for each variable, if any, defined in your sequence.  
+A `Batch` is a group of jobs with the same sequence that will run on the same QPU. For each job of a given batch you must set a value for each variable, if any, defined in your sequence.
 The batch sequence can be generated using [Pulser](https://github.com/pasqal-io/Pulser). See their [documentation](https://pulser.readthedocs.io/en/stable/),
 for more information on how to install the library and create your own sequence.
 
 Once you have created your sequence, you should serialize it as follows:
 
 ```python
 # sequence should be a pulser Sequence object
```

### Comparing `pasqal-cloud-0.3.1/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.3.2/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/sdk/setup.py` & `pasqal-cloud-0.3.2/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/setup.py` & `pasqal-cloud-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,25 +26,24 @@
     include_package_data=True,
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     maintainer="Pasqal Cloud Services",
     maintainer_email="pcs@pasqal.io",
     python_requires=">=3.7",
     license="Apache 2.0",
-    # TODO:
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
     ],
     url="https://github.com/pasqal-io/pasqal-cloud",
     install_requires=[
         "auth0-python >= 3.23.1, <4.0.0 ",
         "requests>=2.25.1, <3.0.0",
         "pyjwt[crypto]>=2.5.0, <3.0.0",
-        "pydantic>=1.10",
+        "pydantic>=1.10, <2.0",
     ],
     extras_require={
         "dev": {
             "black==22.3.0",
             "flake8==3.9.0",
             "flake8-import-order==0.18.1",
             "mypy==0.982",
```

### Comparing `pasqal-cloud-0.3.1/tests/conftest.py` & `pasqal-cloud-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/tests/test_batch.py` & `pasqal-cloud-0.3.2/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/tests/test_client.py` & `pasqal-cloud-0.3.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.3.2/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/tests/test_config.py` & `pasqal-cloud-0.3.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/tests/test_device_specs.py` & `pasqal-cloud-0.3.2/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/tests/test_doubles/authentication.py` & `pasqal-cloud-0.3.2/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/tests/test_job.py` & `pasqal-cloud-0.3.2/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.1/tests/test_project_renaming_compatibility.py` & `pasqal-cloud-0.3.2/tests/test_project_renaming_compatibility.py`

 * *Files identical despite different names*

