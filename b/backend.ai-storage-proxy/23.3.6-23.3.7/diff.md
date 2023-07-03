# Comparing `tmp/backend.ai-storage-proxy-23.3.6.tar.gz` & `tmp/backend.ai-storage-proxy-23.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-23.3.6.tar", last modified: Wed Jun 14 11:13:21 2023, max compression
+gzip compressed data, was "backend.ai-storage-proxy-23.3.7.tar", last modified: Mon Jul  3 16:26:22 2023, max compression
```

## Comparing `backend.ai-storage-proxy-23.3.6.tar` & `backend.ai-storage-proxy-23.3.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/onefs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.469671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/netappclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/subproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/vfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 11:13:21.000000 backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:13:21.473671 backend.ai-storage-proxy-23.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-14 11:13:20.000000 backend.ai-storage-proxy-23.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33435 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.762477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/onefs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/netappclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/vfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:26:22.766477 backend.ai-storage-proxy-23.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-03 16:26:22.000000 backend.ai-storage-proxy-23.3.7/setup.py
```

### Comparing `backend.ai-storage-proxy-23.3.6/PKG-INFO` & `backend.ai-storage-proxy-23.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.6
+Version: 23.3.7
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/abc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
+import logging
 from abc import ABCMeta, abstractmethod
 from pathlib import Path, PurePosixPath
 from typing import (
     Any,
     AsyncIterator,
     Final,
     FrozenSet,
     Mapping,
     Optional,
     Sequence,
     final,
 )
 
-from ai.backend.common.types import BinarySize, HardwareMetadata
+from ai.backend.common.logging import BraceStyleAdapter
+from ai.backend.common.types import BinarySize, HardwareMetadata, QuotaScopeID
 
 from .exception import InvalidSubpathError, VFolderNotFoundError
 from .types import (
     CapacityUsage,
     DirEntry,
     FSPerfMetric,
     QuotaConfig,
@@ -30,58 +32,71 @@
 CAP_VFOLDER: Final = "vfolder"  # ability to create vfolder
 CAP_METRIC: Final = "metric"  # ability to report disk related metrics
 CAP_QUOTA: Final = "quota"  # ability to manage quota limits
 CAP_FAST_FS_SIZE: Final = "fast-fs-size"  # ability to scan filesystem size fast (e.g. by API)
 CAP_FAST_SCAN: Final = "fast-scan"  # ability to scan number of files in vFolder fast (e.g. by API)
 CAP_FAST_SIZE: Final = "fast-size"  # ability to scan vFolder size fast (e.g. by API)
 
+log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
+
 
 class AbstractQuotaModel(metaclass=ABCMeta):
     @abstractmethod
-    def mangle_qspath(self, ref: VFolderID | str | None) -> Path:
+    def mangle_qspath(self, ref: VFolderID | QuotaScopeID | str | None) -> Path:
         raise NotImplementedError
 
     @abstractmethod
     async def create_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         options: Optional[QuotaConfig] = None,
     ) -> None:
         """
         Creates a new quota scope.
 
         Raises `AlreadyExists` error if there is the quota scope with the same name.
         """
         raise NotImplementedError
 
     @abstractmethod
     async def describe_quota_scope(
         self,
-        quota_scope_id: str,
-    ) -> QuotaUsage:
+        quota_scope_id: QuotaScopeID,
+    ) -> Optional[QuotaUsage]:
         """
         Get the information about the given quota scope.
+        Returns None if target quota scope does not exist.
         """
         raise NotImplementedError
 
     @abstractmethod
     async def update_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         options: QuotaConfig,
     ) -> None:
         """
         Update the quota option of the given quota scope.
         """
         raise NotImplementedError
 
     @abstractmethod
+    async def unset_quota(
+        self,
+        quota_scope_id: QuotaScopeID,
+    ) -> None:
+        """
+        Lifts off quota set on given quota scope.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
     async def delete_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
     ) -> None:
         """
         Deletes the given quota scope.
 
         Raises `NotEmpty` error if there are one or more vfolders inside the quota scope.
         """
         raise NotImplementedError
@@ -120,14 +135,15 @@
         """
         raise NotImplementedError
 
     @abstractmethod
     def scan_tree(
         self,
         path: Path,
+        recursive=False,
     ) -> AsyncIterator[DirEntry]:
         """
         Iterates over all files within the given path recursively.
         """
         raise NotImplementedError
 
     @abstractmethod
@@ -223,14 +239,15 @@
     async def get_hwinfo(self) -> HardwareMetadata:
         raise NotImplementedError
 
     @abstractmethod
     async def create_vfolder(
         self,
         vfid: VFolderID,
+        exist_ok=False,
     ) -> None:
         raise NotImplementedError
 
     @abstractmethod
     async def delete_vfolder(self, vfid: VFolderID) -> None:
         raise NotImplementedError
 
@@ -277,15 +294,17 @@
     @abstractmethod
     async def get_used_bytes(self, vfid: VFolderID) -> BinarySize:
         pass
 
     # ------ vfolder operations -------
 
     @abstractmethod
-    def scandir(self, vfid: VFolderID, relpath: PurePosixPath) -> AsyncIterator[DirEntry]:
+    def scandir(
+        self, vfid: VFolderID, relpath: PurePosixPath, recursive=True
+    ) -> AsyncIterator[DirEntry]:
         pass
 
     @abstractmethod
     async def mkdir(
         self,
         vfid: VFolderID,
         relpath: PurePosixPath,
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/api/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,25 @@
 import attr
 import jwt
 import trafaret as t
 from aiohttp import hdrs, web
 
 from ai.backend.common import validators as tx
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import BinarySize
+from ai.backend.common.types import BinarySize, QuotaScopeID
 from ai.backend.storage.exception import ExecutionError
 
 from ..abc import AbstractVolume
 from ..context import Context
-from ..exception import InvalidSubpathError, StorageProxyError, VFolderNotFoundError
+from ..exception import (
+    InvalidSubpathError,
+    QuotaScopeNotFoundError,
+    StorageProxyError,
+    VFolderNotFoundError,
+)
 from ..types import QuotaConfig, VFolderID
 from ..utils import check_params, log_manager_api_entry
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
 @web.middleware
@@ -142,15 +147,15 @@
             data = await volume.get_hwinfo()
             return web.json_response(data)
 
 
 async def create_quota_scope(request: web.Request) -> web.Response:
     class Params(TypedDict):
         volume: str
-        qsid: str
+        qsid: QuotaScopeID
         options: QuotaConfig | None
 
     async with cast(
         AsyncContextManager[Params],
         check_params(
             request,
             t.Dict(
@@ -165,14 +170,103 @@
         await log_manager_api_entry(log, "create_quota_scope", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             await volume.quota_model.create_quota_scope(params["qsid"], params["options"])
             return web.Response(status=204)
 
 
+async def get_quota_scope(request: web.Request) -> web.Response:
+    class Params(TypedDict):
+        volume: str
+        qsid: QuotaScopeID
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("qsid"): tx.QuotaScopeID(),
+                },
+            ),
+        ),
+    ) as params:
+        await log_manager_api_entry(log, "get_quota_scope", params)
+        ctx: Context = request.app["ctx"]
+        async with ctx.get_volume(params["volume"]) as volume:
+            quota_usage = await volume.quota_model.describe_quota_scope(params["qsid"])
+            if not quota_usage:
+                raise QuotaScopeNotFoundError
+            return web.json_response(
+                {
+                    "used_bytes": quota_usage.used_bytes if quota_usage.used_bytes >= 0 else None,
+                    "limit_bytes": (
+                        quota_usage.limit_bytes if quota_usage.limit_bytes >= 0 else None
+                    ),
+                }
+            )
+
+
+async def update_quota_scope(request: web.Request) -> web.Response:
+    class Params(TypedDict):
+        volume: str
+        qsid: QuotaScopeID
+        options: QuotaConfig
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("qsid"): tx.QuotaScopeID(),
+                    t.Key("options"): QuotaConfig.as_trafaret(),
+                },
+            ),
+        ),
+    ) as params:
+        await log_manager_api_entry(log, "update_quota_scope", params)
+        ctx: Context = request.app["ctx"]
+        async with ctx.get_volume(params["volume"]) as volume:
+            quota_usage = await volume.quota_model.describe_quota_scope(params["qsid"])
+            if not quota_usage:
+                await volume.quota_model.create_quota_scope(params["qsid"], params["options"])
+            await volume.quota_model.update_quota_scope(params["qsid"], params["options"])
+            return web.Response(status=204)
+
+
+async def unset_quota(request: web.Request) -> web.Response:
+    class Params(TypedDict):
+        volume: str
+        qsid: QuotaScopeID
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("qsid"): tx.QuotaScopeID(),
+                },
+            ),
+        ),
+    ) as params:
+        await log_manager_api_entry(log, "unset_quota", params)
+        ctx: Context = request.app["ctx"]
+        async with ctx.get_volume(params["volume"]) as volume:
+            quota_usage = await volume.quota_model.describe_quota_scope(params["qsid"])
+            if not quota_usage:
+                raise QuotaScopeNotFoundError
+            await volume.quota_model.unset_quota(params["qsid"])
+            return web.Response(status=204)
+
+
 async def create_vfolder(request: web.Request) -> web.Response:
     class Params(TypedDict):
         volume: str
         vfid: VFolderID
         options: dict[str, Any] | None  # deprecated
 
     async with cast(
@@ -185,17 +279,31 @@
                     t.Key("vfid"): tx.VFolderID(),
                     t.Key("options", default=None): t.Null | t.Dict().allow_extra("*"),
                 },
             ),
         ),
     ) as params:
         await log_manager_api_entry(log, "create_vfolder", params)
+        assert params["vfid"].quota_scope_id is not None
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
-            await volume.create_vfolder(params["vfid"])
+            try:
+                await volume.create_vfolder(params["vfid"])
+            except QuotaScopeNotFoundError:
+                assert params["vfid"].quota_scope_id
+                if initial_max_size_for_quota_scope := (params["options"] or {}).get(
+                    "initial_max_size_for_quota_scope"
+                ):
+                    options = QuotaConfig(initial_max_size_for_quota_scope)
+                else:
+                    options = None
+                await volume.quota_model.create_quota_scope(
+                    params["vfid"].quota_scope_id, options=options
+                )
+                await volume.create_vfolder(params["vfid"])
             return web.Response(status=204)
 
 
 async def delete_vfolder(request: web.Request) -> web.Response:
     class Params(TypedDict):
         volume: str
         vfid: VFolderID
@@ -664,14 +772,15 @@
                             "modified": item.stat.modified.isoformat(),
                         },
                         "symlink_target": item.symlink_target,
                     }
                     async for item in volume.scandir(
                         params["vfid"],
                         params["relpath"],
+                        recursive=False,
                     )
                 ]
         return web.json_response(
             {
                 "items": items,
             },
         )
@@ -879,17 +988,17 @@
         ],
     )
     app["ctx"] = ctx
     app.router.add_route("GET", "/", get_status)
     app.router.add_route("GET", "/volumes", get_volumes)
     app.router.add_route("GET", "/volume/hwinfo", get_hwinfo)
     app.router.add_route("POST", "/quota-scope", create_quota_scope)
-    # TODO: app.router.add_route("GET", "/quota-scope", get_quota_scope)
-    # TODO: app.router.add_route("PATCH", "/quota-scope", update_quota_scope)
-    # TODO: app.router.add_route("DELETE", "/quota-scope", delete_quota_scope)
+    app.router.add_route("GET", "/quota-scope", get_quota_scope)
+    app.router.add_route("PATCH", "/quota-scope", update_quota_scope)
+    app.router.add_route("DELETE", "/quota-scope/quota", unset_quota)
     app.router.add_route("POST", "/folder/create", create_vfolder)
     app.router.add_route("POST", "/folder/delete", delete_vfolder)
     app.router.add_route("POST", "/folder/clone", clone_vfolder)
     app.router.add_route("GET", "/folder/mount", get_vfolder_mount)
     app.router.add_route("GET", "/volume/performance-metric", get_performance_metric)
     app.router.add_route("GET", "/folder/metadata", get_metadata)
     app.router.add_route("POST", "/folder/metadata", set_metadata)
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/cephfs/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 import os
 import shutil
 from pathlib import Path
 from typing import Dict, FrozenSet, List
 
 import aiofiles.os
 
-from ai.backend.common.types import BinarySize
+from ai.backend.common.types import BinarySize, QuotaScopeID
+from ai.backend.storage.exception import QuotaScopeNotFoundError
 
 from ..abc import CAP_FAST_SIZE, CAP_QUOTA, CAP_VFOLDER, AbstractFSOpModel, AbstractQuotaModel
 from ..subproc import run
 from ..types import CapacityUsage, Optional, QuotaConfig, QuotaUsage, TreeUsage
 from ..vfs import BaseFSOpModel, BaseQuotaModel, BaseVolume
 
 
 class CephDirQuotaModel(BaseQuotaModel):
     async def create_quota_scope(
         self,
-        quota_scope_id: str,
-        config: Optional[QuotaConfig] = None,
+        quota_scope_id: QuotaScopeID,
+        options: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         await aiofiles.os.makedirs(qspath)
-        if config is not None:
-            await self.update_quota_scope(quota_scope_id, config)
+        if options is not None:
+            await self.update_quota_scope(quota_scope_id, options)
 
-    async def describe_quota_scope(self, quota_scope_id: str) -> QuotaUsage:
+    async def describe_quota_scope(self, quota_scope_id: QuotaScopeID) -> Optional[QuotaUsage]:
         qspath = self.mangle_qspath(quota_scope_id)
+        if not qspath.exists():
+            return None
         loop = asyncio.get_running_loop()
 
         def read_attrs() -> tuple[int, int]:
             used_bytes = int(os.getxattr(qspath, "ceph.dir.rbytes").decode())  # type: ignore[attr-defined]
             try:
                 limit_bytes = int(os.getxattr(qspath, "ceph.quota.max_bytes").decode())  # type: ignore[attr-defined]
             except OSError as e:
@@ -47,26 +50,42 @@
             None,
             read_attrs,
         )
         return QuotaUsage(used_bytes=used_bytes, limit_bytes=limit_bytes)
 
     async def update_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: QuotaConfig,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
+        if not qspath.exists():
+            raise QuotaScopeNotFoundError
+
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
             # without type: ignore mypy will raise error when trying to run on macOS
             # because os.setxattr() exists only for linux
             lambda: os.setxattr(qspath, "ceph.quota.max_bytes", str(int(config.limit_bytes)).encode()),  # type: ignore[attr-defined]
         )
 
+    async def unset_quota(self, quota_scope_id: QuotaScopeID) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        if not qspath.exists():
+            raise QuotaScopeNotFoundError
+
+        loop = asyncio.get_running_loop()
+        await loop.run_in_executor(
+            None,
+            # without type: ignore mypy will raise error when trying to run on macOS
+            # because os.setxattr() exists only for linux
+            lambda: os.setxattr(qspath, "ceph.quota.max_bytes", b"0"),  # type: ignore[attr-defined]
+        )
+
 
 class CephFSOpModel(BaseFSOpModel):
     async def scan_tree_usage(self, target_path: Path) -> TreeUsage:
         loop = asyncio.get_running_loop()
         raw_reports = await loop.run_in_executor(
             None,
             lambda: (
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/config.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/context.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "xfs": XfsVolume,
     "netapp": NetAppVolume,
     # NOTE: Dell EMC has two different storage: PowerStore and PowerScale (OneFS).
     #       We support the latter only for now.
     "dellemc-onefs": DellEMCOneFSVolume,
     "weka": WekaVolume,
     "gpfs": GPFSVolume,  # IBM SpectrumScale or GPFS
+    "spectrumscale": GPFSVolume,  # IBM SpectrumScale or GPFS
     "cephfs": CephFSVolume,
 }
 
 
 class Context:
     __slots__ = ("pid", "etcd", "local_config", "dsn")
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/__init__.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import FrozenSet, Optional
 
 import aiofiles.os
 
-from ai.backend.common.types import HardwareMetadata
+from ai.backend.common.types import HardwareMetadata, QuotaScopeID
 
 from ..abc import CAP_FAST_FS_SIZE, CAP_METRIC, CAP_QUOTA, CAP_VFOLDER, AbstractQuotaModel
 from ..exception import NotEmptyError
 from ..types import CapacityUsage, FSPerfMetric, QuotaConfig, QuotaUsage
 from ..vfs import BaseQuotaModel, BaseVolume
 from .exceptions import DellNoMetricError
 from .onefs_client import OneFSClient, QuotaThresholds, QuotaTypes
@@ -23,41 +23,41 @@
         api_client: OneFSClient,
     ) -> None:
         super().__init__(mount_path)
         self.api_client = api_client
 
     async def create_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         await aiofiles.os.makedirs(qspath, exist_ok=True)
         if config is not None:
             await self.update_quota_scope(quota_scope_id, config)
 
     async def describe_quota_scope(
         self,
-        quota_scope_id: str,
-    ) -> QuotaUsage:
+        quota_scope_id: QuotaScopeID,
+    ) -> Optional[QuotaUsage]:
         qspath = self.mangle_qspath(quota_scope_id)
         quota_id_path = qspath / ".quota_id"
         if quota_id_path.exists():
             quota_id = quota_id_path.read_text()
             data = await self.api_client.get_quota(quota_id)
             return QuotaUsage(
                 used_bytes=data["usage"]["fslogical"],
                 limit_bytes=data["thresholds"]["hard"],
             )
         else:
-            return QuotaUsage(-1, -1)
+            return None
 
     async def update_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: QuotaConfig,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         quota_id_path = qspath / ".quota_id"
         if quota_id_path.exists():
             quota_id = quota_id_path.read_text()
             await self.api_client.update_quota(
@@ -68,17 +68,30 @@
             result = await self.api_client.create_quota(
                 qspath,
                 QuotaTypes.DIRECTORY,
                 QuotaThresholds(hard=config.limit_bytes, soft=config.limit_bytes),
             )
             quota_id_path.write_text(result["id"])
 
+    async def unset_quota(
+        self,
+        quota_scope_id: QuotaScopeID,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        quota_id_path = qspath / ".quota_id"
+        if len([p for p in qspath.iterdir() if p.is_dir()]) > 0:
+            raise NotEmptyError(quota_scope_id)
+        if quota_id_path.exists():
+            quota_id = quota_id_path.read_text()
+            await self.api_client.delete_quota(quota_id)
+            await aiofiles.os.remove(quota_id_path)
+
     async def delete_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         quota_id_path = qspath / ".quota_id"
         if len([p for p in qspath.iterdir() if p.is_dir()]) > 0:
             raise NotEmptyError(quota_scope_id)
         if quota_id_path.exists():
             quota_id = quota_id_path.read_text()
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/exceptions.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/dellemc/onefs_client.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/dellemc/onefs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
-from typing import Any
+from typing import Any, Optional
 
 from aiohttp import web
+from aiohttp.web_exceptions import HTTPNotFound
 
 
 class StorageProxyError(Exception):
     pass
 
 
 class ExecutionError(StorageProxyError):
@@ -20,14 +21,18 @@
     pass
 
 
 class VFolderNotFoundError(StorageProxyError):
     pass
 
 
+class QuotaScopeNotFoundError(StorageProxyError, HTTPNotFound):
+    pass
+
+
 class InvalidSubpathError(StorageProxyError):
     pass
 
 
 class InvalidQuotaScopeError(StorageProxyError):
     pass
 
@@ -37,15 +42,15 @@
 
 
 class InvalidAPIParameters(web.HTTPBadRequest):
     def __init__(
         self,
         type_suffix: str = "invalid-api-params",
         title: str = "Invalid API parameters",
-        msg: str = None,
+        msg: Optional[str] = None,
         data: Any = None,
     ) -> None:
         payload = {
             "type": f"https://api.backend.ai/probs/storage/{type_suffix}",
             "title": title,
         }
         if msg is not None:
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 from pathlib import Path
 from typing import Any, FrozenSet, Mapping, Optional
 
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import BinarySize, HardwareMetadata
+from ai.backend.common.types import BinarySize, HardwareMetadata, QuotaScopeID
 
 from ..abc import (
     CAP_FAST_FS_SIZE,
     CAP_METRIC,
     CAP_QUOTA,
     CAP_VFOLDER,
     AbstractFSOpModel,
@@ -35,44 +35,50 @@
         super().__init__(mount_path)
         self.api_client = api_client
         self.fs = fs
         self.gpfs_owner = gpfs_owner
 
     async def create_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         await self.api_client.create_fileset(
             self.fs,
-            quota_scope_id,
+            quota_scope_id.pathname,
             path=qspath,
             owner=self.gpfs_owner,
         )
         if config is not None:
             await self.update_quota_scope(quota_scope_id, config)
 
-    async def update_quota_scope(self, quota_scope_id: str, config: QuotaConfig) -> None:
-        await self.api_client.set_quota(self.fs, quota_scope_id, config.limit_bytes)
+    async def update_quota_scope(self, quota_scope_id: QuotaScopeID, config: QuotaConfig) -> None:
+        await self.api_client.set_quota(self.fs, quota_scope_id.pathname, config.limit_bytes)
 
-    async def describe_quota_scope(self, quota_scope_id: str) -> QuotaUsage:
-        quotas = await self.api_client.list_fileset_quotas(self.fs, quota_scope_id)
+    async def describe_quota_scope(self, quota_scope_id: QuotaScopeID) -> Optional[QuotaUsage]:
+        if not self.mangle_qspath(quota_scope_id).exists():
+            return None
+
+        quotas = await self.api_client.list_fileset_quotas(self.fs, quota_scope_id.pathname)
         custom_defined_quotas = [q for q in quotas if not q.defaultQuota]
         if len(custom_defined_quotas) == 0:
             return QuotaUsage(-1, -1)
         quota_info = custom_defined_quotas[0]
         # The units are kilobytes (ref: )
         return QuotaUsage(
             used_bytes=quota_info.blockUsage * 1024 if quota_info.blockUsage is not None else -1,
             limit_bytes=quota_info.blockLimit * 1024 if quota_info.blockLimit is not None else -1,
         )
 
-    async def delete_quota_scope(self, quota_scope_id: str) -> None:
-        await self.api_client.remove_fileset(self.fs, quota_scope_id)
+    async def unset_quota(self, quota_scope_id: QuotaScopeID) -> None:
+        await self.api_client.remove_quota(self.fs, quota_scope_id.pathname)
+
+    async def delete_quota_scope(self, quota_scope_id: QuotaScopeID) -> None:
+        await self.api_client.remove_fileset(self.fs, quota_scope_id.pathname)
 
 
 class GPFSOpModel(BaseFSOpModel):
     def __init__(
         self,
         mount_path: Path,
         scandir_limit: int,
@@ -178,15 +184,15 @@
         free, total = 0, 0
         for _pool in storage_pools:
             pool = await self.api_client.get_fs_pool(self.fs, _pool.storagePoolName)
             if pool.totalDataInKB is None or pool.freeDataInKB is None:
                 continue
             total += pool.totalDataInKB
             free += pool.freeDataInKB
-        return CapacityUsage(BinarySize(total), BinarySize(total - free))
+        return CapacityUsage(BinarySize(total - free) * 1024, BinarySize(total) * 1024)
 
     async def get_performance_metric(self) -> FSPerfMetric:
         # ref: https://www.ibm.com/docs/en/spectrum-scale/5.0.3?topic=2-perfmondata-get
         query = (
             "metrics "
             "avg(gpfs_ns_read_ops),"
             "avg(gpfs_ns_write_ops),"
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
             query = urllib.parse.urlencode({"filter": f"entityType={quota_type}"})
             response = await self._build_request(
                 sess,
                 "GET",
                 f"/filesystems/{fs_name}/filesets/{fileset_name}/quotas?{query}",
             )
             data = await response.json()
+            log.debug("response: {}", data)
         return [GPFSQuota.from_dict(quota_info) for quota_info in data["quotas"]]
 
     @error_handler
     async def set_quota(
         self,
         fs_name: str,
         fileset_name: str,
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/migration.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/migration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import asyncio
 import csv
 import enum
 import logging
 import os
 import re
-import traceback
 from contextlib import asynccontextmanager as actxmgr
 from dataclasses import dataclass
 from io import StringIO
 from pathlib import Path
-from typing import Any, AsyncIterator, Iterator, Optional
+from typing import Any, AsyncIterator, Iterator, Optional, TypedDict
 from uuid import UUID
 
 import aiofiles
 import asyncpg
 import click
 import more_itertools
 import tqdm
@@ -32,14 +31,24 @@
 @dataclass
 class VolumeUpgradeInfo:
     orig_version: int
     target_version: int
     volume: AbstractVolume
 
 
+class MigrationFolderInfo(TypedDict):
+    volume_id: str
+    folder_id: UUID
+    quota_scope_id: str
+    src_path: Path
+    dst_path: Path
+    current_size: Optional[int]
+    old_quota: Optional[int]
+
+
 class VFolderMigrationStatus(enum.StrEnum):
     PENDING = "pending"
     FAILED = "failed"
     COMPLETE = "complete"
 
 
 async def check_latest(ctx: Context) -> list[VolumeUpgradeInfo]:
@@ -77,14 +86,15 @@
     yield conn
     await conn.close()
 
 
 async def upgrade_2_to_3(
     ctx: Context,
     volume: AbstractVolume,
+    outfile: str,
     report_path: Optional[Path] = None,
     force_scan_folder_size: bool = False,
 ) -> None:
     assert ctx.dsn is not None
     rx_two_digits_hex = re.compile(r"^[a-f0-9]{2}$")
     rx_rest_digits_hex = re.compile(r"^[a-f0-9]{28}$")
     log.info("upgrading {} ...", volume.mount_path)
@@ -96,29 +106,17 @@
             if depth < 2:
                 if p.is_dir() and rx_two_digits_hex.search(p.name):
                     yield from scan_vfolders(p, depth=depth + 1)
             else:
                 if p.is_dir() and rx_rest_digits_hex.search(p.name):
                     yield p
 
-    async with connect_database(ctx.dsn) as conn:
-        await conn.execute("""\
-            CREATE TABLE IF NOT EXISTS vfolder_migration_v3 (
-                volume_id VARCHAR(1024),
-                folder_id UUID,
-                status VARCHAR(16),
-                current_size INTEGER DEFAULT NULL,
-                old_quota INTEGER DEFAULT NULL,
-                log TEXT DEFAULT NULL,
-                PRIMARY KEY (volume_id, folder_id)
-            );
-            """)
-
     targets = [*scan_vfolders(volume.mount_path)]
     created_quota_scopes: set[str] = set()
+    migration_informations: list[MigrationFolderInfo] = []
     with tqdm.tqdm(total=len(targets)) as progbar:
         for target_chunk in more_itertools.ichunked(targets, 10):
             folder_ids: list[UUID] = []
             old_quota_map: dict[UUID, Optional[int]] = {}
             quota_scope_map: dict[UUID, str] = {}
             async with connect_database(ctx.dsn) as conn:
                 for target in target_chunk:
@@ -128,212 +126,119 @@
                     """\
                     SELECT "id", "quota_scope_id", "max_size" FROM vfolders
                     WHERE "id" = ANY($1);
                     """,
                     folder_ids,
                 )
                 for row in rows:
-                    old_quota_map[row["id"]] = row["max_size"]
+                    old_quota_map[row["id"]] = (
+                        row["max_size"] * (2**20) if row["max_size"] else None
+                    )
                     quota_scope_map[row["id"]] = row["quota_scope_id"]
 
-                progbar.write("checking {} ...".format(", ".join(map(str, folder_ids))))
-
-                async with conn.transaction():
-                    await conn.executemany(
-                        """\
-                        INSERT INTO vfolder_migration_v3
-                        (volume_id, folder_id, status)
-                        VALUES ($1, $2, $3)
-                        ON CONFLICT (volume_id, folder_id)
-                        DO NOTHING;
-                        """,
-                        [
-                            (
-                                volume_id,
-                                folder_id,
-                                VFolderMigrationStatus.PENDING,
-                            )
-                            for folder_id in folder_ids
-                        ],
-                    )
-
-                rows = await conn.fetch(
-                    """\
-                    SELECT folder_id FROM vfolder_migration_v3
-                    WHERE volume_id = $1
-                      AND folder_id = ANY($2)
-                      AND status = $3;
-                    """,
-                    volume_id,
-                    folder_ids,
-                    VFolderMigrationStatus.COMPLETE,
-                )
-                completed_folder_ids = {row["folder_id"] for row in rows}
+                log.info("checking {} ...".format(", ".join(map(str, folder_ids))))
 
             for folder_id in folder_ids:
-                if folder_id in completed_folder_ids:
-                    progbar.update(1)
+                try:
+                    quota_scope_id = quota_scope_map[folder_id]
+                except KeyError:
                     continue
-                quota_scope_id = quota_scope_map[folder_id]
-                progbar.write(
-                    "moving vfolder {} into quota_scope {}".format(
+                progbar.set_description(
+                    "inspecting contents of vfolder {}".format(
                         folder_id,
-                        quota_scope_id,
                     )
                 )
                 orig_vfid = VFolderID(None, folder_id)
                 dst_vfid = VFolderID(quota_scope_id, folder_id)
                 try:
                     if scan_folder_size:
-                        current_size = await volume.fsop_model.scan_tree_size(
-                            volume.mangle_vfpath(orig_vfid),
+                        current_size = int(
+                            await volume.fsop_model.scan_tree_size(
+                                volume.mangle_vfpath(orig_vfid),
+                            )
                         )
                     else:
                         current_size = None
                     if quota_scope_id not in created_quota_scopes:
-                        await volume.quota_model.create_quota_scope(quota_scope_id)
                         created_quota_scopes.add(quota_scope_id)
-                    await volume.fsop_model.move_tree(
-                        volume.mangle_vfpath(orig_vfid),
-                        volume.mangle_vfpath(dst_vfid),
+                    migration_informations.append(
+                        {
+                            "volume_id": volume_id,
+                            "folder_id": folder_id,
+                            "quota_scope_id": quota_scope_id,
+                            "src_path": volume.mangle_vfpath(orig_vfid),
+                            "dst_path": volume.mangle_vfpath(dst_vfid),
+                            "current_size": current_size,
+                            "old_quota": old_quota_map[folder_id],
+                        }
                     )
                 except Exception:
                     log.exception("error during migration of vfolder {}", folder_id)
-                    async with (
-                        connect_database(ctx.dsn) as conn,
-                        conn.transaction(),
-                    ):
-                        await conn.execute(
-                            """\
-                            INSERT INTO vfolder_migration_v3
-                            (volume_id, folder_id, log, status)
-                            VALUES ($1, $2, $3, $4)
-                            ON CONFLICT (volume_id, folder_id)
-                            DO UPDATE SET log = excluded.log, status = excluded.status;
-                            """,
-                            volume_id,
-                            folder_id,
-                            traceback.format_exc(),
-                            VFolderMigrationStatus.FAILED,
-                        )
-                else:
-                    log.info(
-                        "completed migration of vfolder {}",
-                        folder_id,
-                    )
-                    async with (
-                        connect_database(ctx.dsn) as conn,
-                        conn.transaction(),
-                    ):
-                        if old_quota := old_quota_map[folder_id]:
-                            quota_in_mib = old_quota * (2**20)
-                        else:
-                            quota_in_mib = None
-                        await conn.execute(
-                            """\
-                            INSERT INTO vfolder_migration_v3
-                            (volume_id, folder_id, status, old_quota, current_size)
-                            VALUES ($1, $2, $3, $4, $5)
-                            ON CONFLICT (volume_id, folder_id)
-                            DO UPDATE SET log = NULL, status = excluded.status,
-                            old_quota = excluded.old_quota, current_size = excluded.current_size;
-                            """,
-                            volume_id,
-                            folder_id,
-                            VFolderMigrationStatus.COMPLETE,
-                            quota_in_mib,
-                            int(current_size or 0),
-                        )
-                    await volume.delete_vfolder(orig_vfid)
                 finally:
                     progbar.update(1)
 
-    async with connect_database(ctx.dsn) as conn:
-        incomplete_count = await conn.fetchval(
-            """\
-            SELECT COUNT(*) FROM vfolder_migration_v3
-            WHERE volume_id = $1
-              AND status != $2;
-            """,
-            volume_id,
-            VFolderMigrationStatus.COMPLETE,
-        )
-        if incomplete_count == 0:
-            log.info("successfully upgraded {}", volume.mount_path)
-            (volume.mount_path / "version.txt").write_text("3")
-        else:
-            log.warning(
-                (
-                    "There were {} failed migrations. "
-                    "Check out vfolder_migration_v3 table in the database."
-                ),
-                incomplete_count,
-            )
-            log.warning(
-                "You may re-run the migration to retry the failed ones and remaining vfolders."
-            )
-        if report_path:
-            complete_count = await conn.fetchval(
-                """\
-                SELECT COUNT(*) FROM vfolder_migration_v3
-                WHERE volume_id = $1
-                AND status = $2;
-                """,
-                volume_id,
-                VFolderMigrationStatus.COMPLETE,
-            )
-            in_memory_file = StringIO()
-            fieldnames = ["volume_id", "folder_id", "current_size", "old_quota"]
-            writer = csv.DictWriter(in_memory_file, fieldnames=fieldnames)
-            writer.writeheader()
-            for i in range(0, complete_count, 10):
-                rows = await conn.fetch(
-                    """\
-                    SELECT "volume_id", "folder_id", "current_size", "old_quota" FROM vfolder_migration_v3
-                    WHERE volume_id = $1
-                    AND "status" = $2
-                    ORDER BY "folder_id"
-                    LIMIT 10
-                    OFFSET $3;
-                    """,
-                    volume_id,
-                    VFolderMigrationStatus.COMPLETE,
-                    i,
-                )
-                writer.writerows([dict(x) for x in rows])
+    script = (
+        "#! /bin/sh\n",
+        *[f"mkdir -p {m['dst_path'].parent}\n" for m in migration_informations],
+        *[f"mv {m['src_path']} {m['dst_path']}\n" for m in migration_informations],
+        f"echo 3 > {volume_id}/version.txt\n",
+    )
+    if outfile == "-":
+        print("".join(script))
+    else:
+        file_suffix = str(volume.mount_path).split("/")[-1]
+        async with aiofiles.open(f"{outfile}.{file_suffix}", "w") as fw:
+            await fw.writelines(script)
+    if report_path:
+        in_memory_file = StringIO()
+        fieldnames = [
+            "volume_id",
+            "folder_id",
+            "quota_scope_id",
+            "current_size",
+            "old_quota",
+            "src_path",
+            "dst_path",
+        ]
+        writer = csv.DictWriter(in_memory_file, fieldnames=fieldnames)
+        writer.writeheader()
+        writer.writerows(migration_informations)
 
-            async with aiofiles.open(report_path, "w") as csvfile:
-                await csvfile.write(in_memory_file.getvalue())
+        async with aiofiles.open(report_path, "w") as csvfile:
+            await csvfile.write(in_memory_file.getvalue())
 
 
 upgrade_handlers = {
     3: upgrade_2_to_3,
 }
 
 
 async def check_and_upgrade(
     local_config: dict[str, Any],
     dsn: str,
+    outfile: str,
     report_path: Optional[Path] = None,
     force_scan_folder_size: bool = False,
 ):
     etcd = load_shared_config(local_config)
     ctx = Context(pid=os.getpid(), local_config=local_config, etcd=etcd, dsn=dsn)
     volumes_to_upgrade = await check_latest(ctx)
     for upgrade_info in volumes_to_upgrade:
         handler = upgrade_handlers[upgrade_info.target_version]
         await handler(
             ctx,
             upgrade_info.volume,
+            outfile,
             report_path=report_path,
             force_scan_folder_size=force_scan_folder_size,
         )
 
 
 @click.command()
+@click.argument("outfile")
 @click.option(
     "-f",
     "--config-path",
     "--config",
     type=Path,
     default=None,
     help=(
@@ -373,20 +278,25 @@
 )
 @click.option(
     "--debug",
     is_flag=True,
     help="This option will soon change to --log-level TEXT option.",
 )
 def main(
+    outfile: str,
     config_path: Optional[Path],
     dsn: str,
     report_path: Optional[Path],
     force_scan_folder_size: bool,
     debug: bool,
 ) -> None:
+    """
+    Print migration script to OUTFILE.
+    Pass - as OUTFILE to print results to STDOUT.
+    """
     local_config = load_local_config(config_path, debug=debug)
     ipc_base_path = local_config["storage-proxy"]["ipc-base-path"]
     log_sockpath = Path(
         ipc_base_path / f"storage-proxy-logger-{os.getpid()}.sock",
     )
     log_sockpath.parent.mkdir(parents=True, exist_ok=True)
     log_endpoint = f"ipc://{log_sockpath}"
@@ -397,14 +307,15 @@
         log_endpoint=log_endpoint,
     )
     with logger:
         asyncio.run(
             check_and_upgrade(
                 local_config,
                 dsn,
+                outfile,
                 report_path=report_path,
                 force_scan_folder_size=force_scan_folder_size,
             )
         )
 
 
 if __name__ == "__main__":
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/__init__.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,26 +15,26 @@
     Optional,
 )
 
 import aiofiles
 import aiofiles.os
 
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import BinarySize, HardwareMetadata
+from ai.backend.common.types import BinarySize, HardwareMetadata, QuotaScopeID
 
 from ..abc import (
     CAP_FAST_FS_SIZE,
     CAP_FAST_SIZE,
     CAP_METRIC,
     CAP_QUOTA,
     CAP_VFOLDER,
     AbstractFSOpModel,
     AbstractQuotaModel,
 )
-from ..exception import ExecutionError, NotEmptyError
+from ..exception import ExecutionError, InvalidQuotaScopeError, NotEmptyError
 from ..subproc import spawn_and_watch
 from ..types import (
     SENTINEL,
     CapacityUsage,
     DirEntry,
     DirEntryType,
     FSPerfMetric,
@@ -67,49 +67,57 @@
         super().__init__(mount_path)
         self.netapp_client = netapp_client
         self.svm_id = svm_id
         self.volume_id = volume_id
 
     async def create_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         result = await self.netapp_client.create_qtree(self.svm_id, self.volume_id, qspath.name)
         self.netapp_client.check_job_result(result, [])
         if config is not None:
             await self.update_quota_scope(quota_scope_id, config)
 
     async def describe_quota_scope(
         self,
-        quota_scope_id: str,
-    ) -> QuotaUsage:
+        quota_scope_id: QuotaScopeID,
+    ) -> Optional[QuotaUsage]:
         qspath = self.mangle_qspath(quota_scope_id)
+        if not qspath.exists():
+            return None
         return await self.netapp_client.get_quota_report(self.svm_id, self.volume_id, qspath.name)
 
     async def update_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: QuotaConfig,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         result = await self.netapp_client.set_quota_rule(
             self.svm_id,
             self.volume_id,
             qspath.name,
             config,
         )
         self.netapp_client.check_job_result(result, [])
         result = await self.netapp_client.enable_quota(self.volume_id)
         self.netapp_client.check_job_result(result, ["5308507"])  # pass if "already on"
 
+    # FIXME: How do we implement unset_quota() for NetApp?
+    async def unset_quota(self, quota_scope_id: QuotaScopeID) -> None:
+        raise InvalidQuotaScopeError(
+            "Unsetting folder limit without removing quota scope is not possible for this backend"
+        )
+
     async def delete_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         if len([p for p in qspath.iterdir() if p.is_dir()]) > 0:
             raise NotEmptyError(quota_scope_id)
         # QTree and quota rule is automatically removed
         # when the corresponding directory is deleted.
         await aiofiles.os.rmdir(qspath)
@@ -199,14 +207,15 @@
             async for line in ag:
                 # TODO: line for bgtask
                 pass
 
     def scan_tree(
         self,
         target_path: Path,
+        recursive=False,
     ) -> AsyncIterator[DirEntry]:
         target_relpath = target_path.relative_to(self.mount_path)
         nfspath = f"{self.netapp_nfs_host}:{self.nas_path}/{target_relpath}"
         # Use a custom formatting
         scan_cmd = [
             *self.netapp_xcp_cmd,
             b"scan",
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/netapp/netappclient.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/netapp/netappclient.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             )
         except CalledProcessError as e:
             raise RuntimeError(f"'prm' command failed: {e.stderr}")
 
     def scan_tree(
         self,
         target_path: Path,
+        recursive=False,
     ) -> AsyncIterator[DirEntry]:
         raw_target_path = os.fsencode(target_path)
 
         async def _aiter() -> AsyncIterator[DirEntry]:
             proc = await asyncio.create_subprocess_exec(
                 b"pls",
                 b"--json",
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/server.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/subproc.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/subproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/types.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/vfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,25 @@
 from pathlib import Path, PurePosixPath
 from typing import AsyncIterator, FrozenSet, Optional, Sequence, Union, final
 
 import aiofiles.os
 import janus
 import trafaret as t
 
-from ai.backend.common import validators as tx
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import BinarySize, HardwareMetadata
+from ai.backend.common.types import BinarySize, HardwareMetadata, QuotaScopeID
 
 from ..abc import CAP_VFOLDER, AbstractFSOpModel, AbstractQuotaModel, AbstractVolume
-from ..exception import ExecutionError, InvalidAPIParameters, InvalidQuotaScopeError, NotEmptyError
+from ..exception import (
+    ExecutionError,
+    InvalidAPIParameters,
+    InvalidQuotaScopeError,
+    NotEmptyError,
+    QuotaScopeNotFoundError,
+)
 from ..subproc import run
 from ..types import (
     SENTINEL,
     CapacityUsage,
     DirEntry,
     DirEntryType,
     FSPerfMetric,
@@ -47,63 +52,74 @@
     to split vfolders into per-user/per-project namespaces, without
     imposing any actual quota limits.
     """
 
     def __init__(self, mount_path: Path) -> None:
         self.mount_path = mount_path
 
-    def mangle_qspath(self, ref: VFolderID | str | None) -> Path:
+    def mangle_qspath(self, ref: VFolderID | QuotaScopeID | str | None) -> Path:
         try:
             match ref:
                 case VFolderID():
                     if ref.quota_scope_id is None:
                         return self.mount_path  # for legacy vfolder paths during migration
-                    tx.QuotaScopeID().check(ref.quota_scope_id)
-                    return Path(self.mount_path, ref.quota_scope_id)
+                    return Path(self.mount_path, ref.quota_scope_id.pathname)
+                case QuotaScopeID():
+                    return Path(self.mount_path, ref.pathname)
                 case str():
-                    tx.QuotaScopeID().check(ref)
-                    return Path(self.mount_path, ref)
+                    typed_scope_id = QuotaScopeID.parse(ref)
+                    return Path(self.mount_path, typed_scope_id.pathname)
                 case None:
                     return self.mount_path  # for legacy vfolder paths during migration
                 case _:
                     raise InvalidQuotaScopeError(
                         f"Invalid value format for quota scope ID: {ref!r}"
                     )
         except t.DataError:
             raise InvalidQuotaScopeError(f"Invalid value format for quota scope ID: {ref!r}")
 
     async def create_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
             lambda: qspath.mkdir(0o755, parents=True, exist_ok=False),
         )
 
     async def describe_quota_scope(
         self,
-        quota_scope_id: str,
-    ) -> QuotaUsage:
+        quota_scope_id: QuotaScopeID,
+    ) -> Optional[QuotaUsage]:
+        if not self.mangle_qspath(quota_scope_id).exists():
+            return None
+
         return QuotaUsage(-1, -1)
 
     async def update_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         options: QuotaConfig,
     ) -> None:
         # This is a no-op.
         pass
 
+    async def unset_quota(
+        self,
+        quota_scope_id: QuotaScopeID,
+    ) -> None:
+        # This is a no-op.
+        pass
+
     async def delete_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         if len([p for p in qspath.iterdir() if p.is_dir()]) > 0:
             raise NotEmptyError(quota_scope_id)
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
@@ -116,43 +132,52 @@
     This quota model uses the Linux's vanilla gid-based quota scheme
     with setgid on the first-level namespace directories for each user
     or each project.
     """
 
     async def create_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
             lambda: qspath.mkdir(0o755, parents=True, exist_ok=False),
         )
         # TODO: setgid impl.
 
     async def describe_quota_scope(
         self,
-        quota_scope_id: str,
-    ) -> QuotaUsage:
+        quota_scope_id: QuotaScopeID,
+    ) -> Optional[QuotaUsage]:
+        if not self.mangle_qspath(quota_scope_id).exists():
+            return None
         # TODO: setgid impl.
         return QuotaUsage(-1, -1)
 
     async def update_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         options: QuotaConfig,
     ) -> None:
         # TODO: setgid impl.
         raise NotImplementedError
 
+    async def unset_quota(
+        self,
+        quota_scope_id: QuotaScopeID,
+    ) -> None:
+        # TODO: setgid impl.
+        raise NotImplementedError
+
     async def delete_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         if len([p for p in qspath.iterdir() if p.is_dir()]) > 0:
             raise NotEmptyError(quota_scope_id)
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
@@ -202,27 +227,30 @@
             await loop.run_in_executor(None, functools.partial(shutil.rmtree, path))
         except FileNotFoundError:
             pass
 
     def scan_tree(
         self,
         target_path: Path,
+        recursive: bool = True,
     ) -> AsyncIterator[DirEntry]:
         q: janus.Queue[Sentinel | DirEntry] = janus.Queue()
         loop = asyncio.get_running_loop()
 
         def _scandir(target_path: Path, q: janus._SyncQueueProxy[Sentinel | DirEntry]) -> None:
             count = 0
             limit = self.scandir_limit
             next_paths: deque[Path] = deque()
             next_paths.append(target_path)
             while next_paths:
                 next_path = next_paths.popleft()
                 with os.scandir(next_path) as scanner:
                     for entry in scanner:
+                        if limit > 0 and count == limit:
+                            break
                         symlink_target = ""
                         entry_type = DirEntryType.FILE
                         try:
                             if entry.is_dir():
                                 entry_type = DirEntryType.DIRECTORY
                             if entry.is_symlink():
                                 entry_type = DirEntryType.SYMLINK
@@ -246,19 +274,17 @@
                                 mode=entry_stat.st_mode,
                                 modified=fstime2datetime(entry_stat.st_mtime),
                                 created=fstime2datetime(entry_stat.st_ctime),
                             ),
                             symlink_target=symlink_target,
                         )
                         q.put(item)
-                        if entry.is_dir() and not entry.is_symlink():
+                        if recursive and entry.is_dir() and not entry.is_symlink():
                             next_paths.append(Path(entry.path))
                         count += 1
-                        if limit > 0 and count == limit:
-                            break
 
         async def _scan_task(q: janus.Queue[Sentinel | DirEntry]) -> None:
             try:
                 await loop.run_in_executor(None, _scandir, target_path, q.sync_q)
             finally:
                 await q.async_q.put(SENTINEL)
 
@@ -350,22 +376,21 @@
             "metadata": {},
         }
 
     @final
     async def create_vfolder(
         self,
         vfid: VFolderID,
+        exist_ok=False,
     ) -> None:
         qspath = self.quota_model.mangle_qspath(vfid)
         if not qspath.exists():
-            raise InvalidQuotaScopeError(
-                f"Quota scope {qspath} does not exist in the target volume"
-            )
+            raise QuotaScopeNotFoundError
         vfpath = self.mangle_vfpath(vfid)
-        await aiofiles.os.makedirs(vfpath, 0o755)
+        await aiofiles.os.makedirs(vfpath, 0o755, exist_ok=exist_ok)
 
     @final
     async def delete_vfolder(self, vfid: VFolderID) -> None:
         vfpath = self.mangle_vfpath(vfid)
         await self.fsop_model.delete_tree(vfpath)
         for p in [vfpath, vfpath.parent, vfpath.parent.parent]:
             try:
@@ -453,17 +478,19 @@
     async def get_used_bytes(self, vfid: VFolderID) -> BinarySize:
         vfpath = self.mangle_vfpath(vfid)
         return await self.fsop_model.scan_tree_size(vfpath)
 
     # ------ vfolder internal operations -------
 
     @final
-    def scandir(self, vfid: VFolderID, relpath: PurePosixPath) -> AsyncIterator[DirEntry]:
+    def scandir(
+        self, vfid: VFolderID, relpath: PurePosixPath, recursive=True
+    ) -> AsyncIterator[DirEntry]:
         target_path = self.sanitize_vfpath(vfid, relpath)
-        return self.fsop_model.scan_tree(target_path)
+        return self.fsop_model.scan_tree(target_path, recursive=recursive)
 
     async def mkdir(
         self,
         vfid: VFolderID,
         relpath: PurePosixPath,
         *,
         parents: bool = False,
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Any, FrozenSet, Mapping, Optional
 
 import aiofiles.os
 
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import HardwareMetadata, QuotaConfig
+from ai.backend.common.types import HardwareMetadata, QuotaConfig, QuotaScopeID
 
 from ..abc import CAP_FAST_FS_SIZE, CAP_METRIC, CAP_QUOTA, CAP_VFOLDER, AbstractQuotaModel
 from ..types import CapacityUsage, FSPerfMetric, QuotaUsage
 from ..vfs import BaseQuotaModel, BaseVolume
 from .exceptions import WekaAPIError, WekaInitError, WekaNoMetricError, WekaNotFoundError
 from .weka_client import WekaAPIClient
 
@@ -36,41 +36,52 @@
         return await loop.run_in_executor(
             None,
             lambda: os.stat(path).st_ino,
         )
 
     async def create_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         await aiofiles.os.makedirs(qspath)
         assert self.fs_uid is not None
         if config is not None:
             await self.update_quota_scope(quota_scope_id, config)
 
-    async def update_quota_scope(self, quota_scope_id: str, config: QuotaConfig) -> None:
+    async def update_quota_scope(self, quota_scope_id: QuotaScopeID, config: QuotaConfig) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         inode_id = await self._get_inode_id(qspath)
         qs_relpath = qspath.relative_to(self.mount_path).as_posix()
         if not qs_relpath.startswith("/"):
             qs_relpath = "/" + qs_relpath
         await self.api_client.set_quota_v1(qs_relpath, inode_id, hard_limit=config.limit_bytes)
 
-    async def describe_quota_scope(self, quota_scope_id: str) -> QuotaUsage:
+    async def describe_quota_scope(self, quota_scope_id: QuotaScopeID) -> Optional[QuotaUsage]:
         qspath = self.mangle_qspath(quota_scope_id)
+        if not qspath.exists():
+            return None
+
         inode_id = await self._get_inode_id(qspath)
         quota = await self.api_client.get_quota(self.fs_uid, inode_id)
         return QuotaUsage(
             used_bytes=quota.used_bytes if quota.used_bytes is not None else -1,
             limit_bytes=quota.hard_limit if quota.hard_limit is not None else -1,
         )
 
-    async def delete_quota_scope(self, quota_scope_id: str) -> None:
+    async def unset_quota(self, quota_scope_id: QuotaScopeID) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        inode_id = await self._get_inode_id(qspath)
+        try:
+            await self.api_client.remove_quota(self.fs_uid, inode_id)
+        except WekaNotFoundError:
+            pass
+
+    async def delete_quota_scope(self, quota_scope_id: QuotaScopeID) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         inode_id = await self._get_inode_id(qspath)
         try:
             await self.api_client.remove_quota(self.fs_uid, inode_id)
         except WekaNotFoundError:
             pass
         await aiofiles.os.rmdir(qspath)
```

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/weka/weka_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-23.3.7/ai/backend/storage/xfs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 )
 
 import aiofiles
 import aiofiles.os
 
 from ai.backend.common.lock import FileLock
 from ai.backend.common.logging import BraceStyleAdapter
+from ai.backend.common.types import QuotaScopeID
 from ai.backend.storage.abc import CAP_QUOTA, CAP_VFOLDER
 
 from ..abc import AbstractQuotaModel
-from ..exception import NotEmptyError
+from ..exception import InvalidQuotaScopeError, NotEmptyError
 from ..subproc import run
 from ..types import (
     QuotaConfig,
     QuotaUsage,
 )
 from ..vfs import BaseQuotaModel, BaseVolume
 
@@ -61,15 +62,15 @@
         else:
             await run(["sudo", "touch", self.file_projid])
         if not Path(self.file_projects).is_file():
             await run(["sudo", "touch", self.file_projects])
 
     async def add_project_entry(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         qspath: Path,
         *,
         project_id: Optional[int] = None,
     ) -> None:
         if project_id is None:
             project_id = self.get_free_project_id()
 
@@ -89,15 +90,15 @@
                 _projects_content += f"{project_id}:{qspath}\n"
                 _tmp_projects.write(_projects_content.encode("ascii"))
                 temp_name_projects = _tmp_projects.name
 
                 _projid_content = Path(self.file_projid).read_text()
                 if _projid_content.strip() != "" and not _projid_content.endswith("\n"):
                     _projid_content += "\n"
-                _projid_content += f"{quota_scope_id}:{project_id}\n"
+                _projid_content += f"{quota_scope_id.pathname}:{project_id}\n"
                 _tmp_projid.write(_projid_content.encode("ascii"))
                 temp_name_projid = _tmp_projid.name
             finally:
                 _tmp_projects.close()
                 _tmp_projid.close()
 
         def _delete_temp_files():
@@ -114,17 +115,17 @@
         try:
             await loop.run_in_executor(None, _create_temp_files)
             await run(["sudo", "cp", "-rp", temp_name_projects, self.file_projects])
             await run(["sudo", "cp", "-rp", temp_name_projid, self.file_projid])
         finally:
             await loop.run_in_executor(None, _delete_temp_files)
 
-    async def remove_project_entry(self, quota_scope_id: str) -> None:
-        await run(["sudo", "sed", "-i.bak", f"/{quota_scope_id}/d", self.file_projects])
-        await run(["sudo", "sed", "-i.bak", f"/{quota_scope_id}/d", self.file_projid])
+    async def remove_project_entry(self, quota_scope_id: QuotaScopeID) -> None:
+        await run(["sudo", "sed", "-i.bak", f"/{quota_scope_id.pathname}/d", self.file_projects])
+        await run(["sudo", "sed", "-i.bak", f"/{quota_scope_id.pathname}/d", self.file_projid])
 
     def get_free_project_id(self) -> int:
         """
         Get the next project_id, which is the smallest unused integer.
         """
         project_id = -1
         for i in range(len(self.project_id_pool) - 1):
@@ -151,15 +152,15 @@
         super().__init__(mount_path)
         self.project_registry = project_registry
         stat_vfs = os.statvfs(mount_path)
         self.block_size = stat_vfs.f_bsize
 
     async def create_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: Optional[QuotaConfig] = None,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         try:
             if config is None:
                 # Set the limit as the filesystem size
                 vfs_stat = os.statvfs(self.mount_path)
@@ -177,68 +178,78 @@
             log.exception("quota-scope creation error")
             raise
         if config is not None:
             await self.update_quota_scope(quota_scope_id, config)
 
     async def describe_quota_scope(
         self,
-        quota_scope_id: str,
-    ) -> QuotaUsage:
+        quota_scope_id: QuotaScopeID,
+    ) -> Optional[QuotaUsage]:
+        if not self.mangle_qspath(quota_scope_id).exists():
+            return None
         full_report = await run(
             # -p: project quota only
             # -b: as number of blocks
             # -N: without header
             ["sudo", "xfs_quota", "-x", "-c", "report -p -b -N", self.mount_path],
         )
         print(full_report)
         for line in full_report.splitlines():
-            if quota_scope_id in line:
+            if quota_scope_id.pathname in line:
                 report = line
                 break
         else:
-            raise RuntimeError(f"unknown xfs project ID: {quota_scope_id}")
+            raise RuntimeError(f"unknown xfs project ID: {quota_scope_id.pathname}")
         if len(report.split()) != 6:
             raise ValueError("unexpected format for xfs_quota report")
         _, used_kbs, _, hard_limit_kbs, _, _ = report.split()
         # By default, report command displays the sizes in the 1 KiB unit.
         used_bytes = int(used_kbs) * 1024
         hard_limit_bytes = int(hard_limit_kbs) * 1024
         return QuotaUsage(used_bytes, hard_limit_bytes)
 
     async def update_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
         config: QuotaConfig,
     ) -> None:
         # This will annotate all entries under the quota scope tree as a part of the project.
         await run(
             [
                 "sudo",
                 "xfs_quota",
                 "-x",
                 "-c",
-                f"project -s {quota_scope_id}",
+                f"project -s {quota_scope_id.pathname}",
                 self.mount_path,
             ],
         )
         # bsoft, bhard accepts bytes or binary-prefixed numbers.
         await run(
             [
                 "sudo",
                 "xfs_quota",
                 "-x",
                 "-c",
-                f"limit -p bsoft={config.limit_bytes} bhard={config.limit_bytes} {quota_scope_id}",
+                (
+                    "limit -p"
+                    f" bsoft={config.limit_bytes} bhard={config.limit_bytes} {quota_scope_id.pathname}"
+                ),
                 self.mount_path,
             ],
         )
 
+    async def unset_quota(self, quota_scope_id: QuotaScopeID) -> None:
+        raise InvalidQuotaScopeError(
+            "Unsetting folder limit without removing quota scope is not possible for this backend"
+        )
+
     async def delete_quota_scope(
         self,
-        quota_scope_id: str,
+        quota_scope_id: QuotaScopeID,
     ) -> None:
         qspath = self.mangle_qspath(quota_scope_id)
         if len([p for p in qspath.iterdir() if p.is_dir()]) > 0:
             raise NotEmptyError(quota_scope_id)
         async with FileLock(LOCK_FILE):
             await self.project_registry.read_project_info()
             await self.project_registry.remove_project_entry(quota_scope_id)
```

### Comparing `backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.6
+Version: 23.3.7
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.6/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-23.3.7/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/backend_shim.py` & `backend.ai-storage-proxy-23.3.7/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.6/setup.py` & `backend.ai-storage-proxy-23.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'asyncpg>=0.27.0',
         'attrs>=20.3',
-        """backend.ai-common==23.03.6
+        """backend.ai-common==23.03.7
 """,
         'click>=7.1.2',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
         'more-itertools~=8.13.0',
         'setproctitle~=1.3.2',
         'tenacity>=8.0',
@@ -250,11 +250,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.6
+    'version': """23.03.7
 """,
     'zip_safe': False,
 })
```

