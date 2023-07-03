# Comparing `tmp/Aruna-Python-API-1.1.0rc7.tar.gz` & `tmp/Aruna-Python-API-1.1.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aruna-Python-API-1.1.0rc7.tar", last modified: Fri Jun 30 12:19:08 2023, max compression
+gzip compressed data, was "Aruna-Python-API-1.1.0rc8.tar", last modified: Mon Jul  3 07:56:47 2023, max compression
```

## Comparing `Aruna-Python-API-1.1.0rc7.tar` & `Aruna-Python-API-1.1.0rc8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.603444 Aruna-Python-API-1.1.0rc7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.591443 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 12:19:08.000000 Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-30 12:19:08.603444 Aruna-Python-API-1.1.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.591443 Aruna-Python-API-1.1.0rc7/aruna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.591443 Aruna-Python-API-1.1.0rc7/aruna/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.591443 Aruna-Python-API-1.1.0rc7/aruna/api/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/notification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21174 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.595443 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 12:19:08.599444 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 12:18:39.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25264 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-30 12:19:08.603444 Aruna-Python-API-1.1.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-30 12:18:56.000000 Aruna-Python-API-1.1.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.338377 Aruna-Python-API-1.1.0rc8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.322377 Aruna-Python-API-1.1.0rc8/Aruna_Python_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-03 07:56:47.000000 Aruna-Python-API-1.1.0rc8/Aruna_Python_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-03 07:56:47.000000 Aruna-Python-API-1.1.0rc8/Aruna_Python_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 07:56:47.000000 Aruna-Python-API-1.1.0rc8/Aruna_Python_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-03 07:56:47.000000 Aruna-Python-API-1.1.0rc8/Aruna_Python_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 07:56:47.000000 Aruna-Python-API-1.1.0rc8/Aruna_Python_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-03 07:56:47.338377 Aruna-Python-API-1.1.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.322377 Aruna-Python-API-1.1.0rc8/aruna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.322377 Aruna-Python-API-1.1.0rc8/aruna/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.326377 Aruna-Python-API-1.1.0rc8/aruna/api/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.326377 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/authorize_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/authorize_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/authorize_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/bundler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/bundler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/bundler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/notification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/notification_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/notification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/proxy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/proxy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/proxy_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.326377 Aruna-Python-API-1.1.0rc8/aruna/api/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.326377 Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.330377 Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/v1/notification_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/v1/notification_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.330377 Aruna-Python-API-1.1.0rc8/aruna/api/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.330377 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.330377 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/auth_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/models_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21174 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/models_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/models_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/query_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/query_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/query_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.330377 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:47.334377 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:56:22.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/collection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/collection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/info_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/info_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/info_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/object_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25264 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/object_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/object_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/objectgroup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/project_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/project_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/service_account_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 07:56:47.338377 Aruna-Python-API-1.1.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-03 07:56:36.000000 Aruna-Python-API-1.1.0rc8/setup.py
```

### Comparing `Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/PKG-INFO` & `Aruna-Python-API-1.1.0rc8/Aruna_Python_API.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc7
+Version: 1.1.0rc8
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc7/Aruna_Python_API.egg-info/SOURCES.txt` & `Aruna-Python-API-1.1.0rc8/Aruna_Python_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/LICENSE` & `Aruna-Python-API-1.1.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/PKG-INFO` & `Aruna-Python-API-1.1.0rc8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc7
+Version: 1.1.0rc8
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc7/README.md` & `Aruna-Python-API-1.1.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/authorize_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/authorize_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/authorize_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/authorize_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/bundler_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/bundler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/bundler_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/bundler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/notification_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/proxy_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/proxy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/internal/v1/proxy_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/internal/v1/proxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/v1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/v1/notification_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/notification/services/v1/notification_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/notification/services/v1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/auth_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&aruna/api/storage/models/v1/auth.proto\x12\x1b\x61runa.api.storage.models.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xd1\x01\n\x07Project\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12Y\n\x10user_permissions\x18\x03 \x03(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\x12%\n\x0e\x63ollection_ids\x18\x04 \x03(\tR\rcollectionIds\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\"\x99\x01\n\x0fProjectOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12%\n\x0e\x63ollection_ids\x18\x04 \x03(\tR\rcollectionIds\x12\x19\n\x08user_ids\x18\x05 \x03(\tR\x07userIds\"\xd1\x01\n\x04User\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1f\n\x0b\x65xternal_id\x18\x02 \x01(\tR\nexternalId\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\x12,\n\x12is_service_account\x18\x06 \x01(\x08R\x10isServiceAccount\x12\x14\n\x05\x65mail\x18\x07 \x01(\tR\x05\x65mail\"\xc9\x03\n\x05Token\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x45\n\ntoken_type\x18\x04 \x01(\x0e\x32&.aruna.api.storage.models.v1.TokenTypeR\ttokenType\x12\x39\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\x12#\n\rcollection_id\x18\x07 \x01(\tR\x0c\x63ollectionId\x12\x1d\n\nproject_id\x18\x08 \x01(\tR\tprojectId\x12G\n\npermission\x18\t \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12\x1d\n\nis_session\x18\n \x01(\x08R\tisSession\x12\x33\n\x07used_at\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x06usedAt\"\xbd\x01\n\x11ProjectPermission\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12\'\n\x0fservice_account\x18\x04 \x01(\x08R\x0eserviceAccount\"\xc2\x01\n\x1cProjectPermissionDisplayName\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12!\n\x0c\x64isplay_name\x18\x04 \x01(\tR\x0b\x64isplayName*\x96\x01\n\nPermission\x12\x1a\n\x16PERMISSION_UNSPECIFIED\x10\x00\x12\x13\n\x0fPERMISSION_NONE\x10\x01\x12\x13\n\x0fPERMISSION_READ\x10\x02\x12\x15\n\x11PERMISSION_APPEND\x10\x03\x12\x15\n\x11PERMISSION_MODIFY\x10\x04\x12\x14\n\x10PERMISSION_ADMIN\x10\x05*g\n\x08PermType\x12\x19\n\x15PERM_TYPE_UNSPECIFIED\x10\x00\x12\x12\n\x0ePERM_TYPE_USER\x10\x01\x12\x17\n\x13PERM_TYPE_ANONYMOUS\x10\x02\x12\x13\n\x0fPERM_TYPE_TOKEN\x10\x03*W\n\tTokenType\x12\x1a\n\x16TOKEN_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13TOKEN_TYPE_PERSONAL\x10\x01\x12\x15\n\x11TOKEN_TYPE_SCOPED\x10\x02\x42<Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&aruna/api/storage/models/v1/auth.proto\x12\x1b\x61runa.api.storage.models.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xe7\x01\n\x07Project\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12Y\n\x10user_permissions\x18\x03 \x03(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\x12%\n\x0e\x63ollection_ids\x18\x04 \x03(\tR\rcollectionIds\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x14\n\x05\x66lags\x18\x06 \x01(\x03R\x05\x66lags\"\xaf\x01\n\x0fProjectOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12%\n\x0e\x63ollection_ids\x18\x04 \x03(\tR\rcollectionIds\x12\x19\n\x08user_ids\x18\x05 \x03(\tR\x07userIds\x12\x14\n\x05\x66lags\x18\x06 \x01(\x03R\x05\x66lags\"\xd1\x01\n\x04User\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1f\n\x0b\x65xternal_id\x18\x02 \x01(\tR\nexternalId\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\x12,\n\x12is_service_account\x18\x06 \x01(\x08R\x10isServiceAccount\x12\x14\n\x05\x65mail\x18\x07 \x01(\tR\x05\x65mail\"\xc9\x03\n\x05Token\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x45\n\ntoken_type\x18\x04 \x01(\x0e\x32&.aruna.api.storage.models.v1.TokenTypeR\ttokenType\x12\x39\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\x12#\n\rcollection_id\x18\x07 \x01(\tR\x0c\x63ollectionId\x12\x1d\n\nproject_id\x18\x08 \x01(\tR\tprojectId\x12G\n\npermission\x18\t \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12\x1d\n\nis_session\x18\n \x01(\x08R\tisSession\x12\x33\n\x07used_at\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x06usedAt\"\xbd\x01\n\x11ProjectPermission\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12\'\n\x0fservice_account\x18\x04 \x01(\x08R\x0eserviceAccount\"\xc2\x01\n\x1cProjectPermissionDisplayName\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12!\n\x0c\x64isplay_name\x18\x04 \x01(\tR\x0b\x64isplayName*\x96\x01\n\nPermission\x12\x1a\n\x16PERMISSION_UNSPECIFIED\x10\x00\x12\x13\n\x0fPERMISSION_NONE\x10\x01\x12\x13\n\x0fPERMISSION_READ\x10\x02\x12\x15\n\x11PERMISSION_APPEND\x10\x03\x12\x15\n\x11PERMISSION_MODIFY\x10\x04\x12\x14\n\x10PERMISSION_ADMIN\x10\x05*g\n\x08PermType\x12\x19\n\x15PERM_TYPE_UNSPECIFIED\x10\x00\x12\x12\n\x0ePERM_TYPE_USER\x10\x01\x12\x17\n\x13PERM_TYPE_ANONYMOUS\x10\x02\x12\x13\n\x0fPERM_TYPE_TOKEN\x10\x03*W\n\tTokenType\x12\x1a\n\x16TOKEN_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13TOKEN_TYPE_PERSONAL\x10\x01\x12\x15\n\x11TOKEN_TYPE_SCOPED\x10\x02\x42<Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.models.v1.auth_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1'
-  _PERMISSION._serialized_start=1534
-  _PERMISSION._serialized_end=1684
-  _PERMTYPE._serialized_start=1686
-  _PERMTYPE._serialized_end=1789
-  _TOKENTYPE._serialized_start=1791
-  _TOKENTYPE._serialized_end=1878
+  _PERMISSION._serialized_start=1578
+  _PERMISSION._serialized_end=1728
+  _PERMTYPE._serialized_start=1730
+  _PERMTYPE._serialized_end=1833
+  _TOKENTYPE._serialized_start=1835
+  _TOKENTYPE._serialized_end=1922
   _PROJECT._serialized_start=105
-  _PROJECT._serialized_end=314
-  _PROJECTOVERVIEW._serialized_start=317
-  _PROJECTOVERVIEW._serialized_end=470
-  _USER._serialized_start=473
-  _USER._serialized_end=682
-  _TOKEN._serialized_start=685
-  _TOKEN._serialized_end=1142
-  _PROJECTPERMISSION._serialized_start=1145
-  _PROJECTPERMISSION._serialized_end=1334
-  _PROJECTPERMISSIONDISPLAYNAME._serialized_start=1337
-  _PROJECTPERMISSIONDISPLAYNAME._serialized_end=1531
+  _PROJECT._serialized_end=336
+  _PROJECTOVERVIEW._serialized_start=339
+  _PROJECTOVERVIEW._serialized_end=514
+  _USER._serialized_start=517
+  _USER._serialized_end=726
+  _TOKEN._serialized_start=729
+  _TOKEN._serialized_end=1186
+  _PROJECTPERMISSION._serialized_start=1189
+  _PROJECTPERMISSION._serialized_end=1378
+  _PROJECTPERMISSIONDISPLAYNAME._serialized_start=1381
+  _PROJECTPERMISSIONDISPLAYNAME._serialized_end=1575
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/auth_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/auth_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -17,40 +17,44 @@
 PERM_TYPE_UNSPECIFIED: PermType
 PERM_TYPE_USER: PermType
 TOKEN_TYPE_PERSONAL: TokenType
 TOKEN_TYPE_SCOPED: TokenType
 TOKEN_TYPE_UNSPECIFIED: TokenType
 
 class Project(_message.Message):
-    __slots__ = ["collection_ids", "description", "id", "name", "user_permissions"]
+    __slots__ = ["collection_ids", "description", "flags", "id", "name", "user_permissions"]
     COLLECTION_IDS_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    FLAGS_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     USER_PERMISSIONS_FIELD_NUMBER: _ClassVar[int]
     collection_ids: _containers.RepeatedScalarFieldContainer[str]
     description: str
+    flags: int
     id: str
     name: str
     user_permissions: _containers.RepeatedCompositeFieldContainer[ProjectPermission]
-    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., user_permissions: _Optional[_Iterable[_Union[ProjectPermission, _Mapping]]] = ..., collection_ids: _Optional[_Iterable[str]] = ..., description: _Optional[str] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., user_permissions: _Optional[_Iterable[_Union[ProjectPermission, _Mapping]]] = ..., collection_ids: _Optional[_Iterable[str]] = ..., description: _Optional[str] = ..., flags: _Optional[int] = ...) -> None: ...
 
 class ProjectOverview(_message.Message):
-    __slots__ = ["collection_ids", "description", "id", "name", "user_ids"]
+    __slots__ = ["collection_ids", "description", "flags", "id", "name", "user_ids"]
     COLLECTION_IDS_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    FLAGS_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     USER_IDS_FIELD_NUMBER: _ClassVar[int]
     collection_ids: _containers.RepeatedScalarFieldContainer[str]
     description: str
+    flags: int
     id: str
     name: str
     user_ids: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., collection_ids: _Optional[_Iterable[str]] = ..., user_ids: _Optional[_Iterable[str]] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., collection_ids: _Optional[_Iterable[str]] = ..., user_ids: _Optional[_Iterable[str]] = ..., flags: _Optional[int] = ...) -> None: ...
 
 class ProjectPermission(_message.Message):
     __slots__ = ["permission", "project_id", "service_account", "user_id"]
     PERMISSION_FIELD_NUMBER: _ClassVar[int]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
     USER_ID_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/models_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/models_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/models/v1/query_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/models/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/collection_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/collection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/endpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/endpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/info_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/info_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/info_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/info_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/object_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/object_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/object_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/object_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/objectgroup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/project_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 
 from aruna.api.storage.models.v1 import auth_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_auth__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.7*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"`\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04\x66lag\x18\x03 \x01(\x03R\x04\x66lag\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"\x7f\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04\x66lag\x18\x04 \x01(\x03R\x04\x66lag\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.8*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.project_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.7*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
+  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.8*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
   _PROJECTSERVICE.methods_by_name['CreateProject']._options = None
   _PROJECTSERVICE.methods_by_name['CreateProject']._serialized_options = b'\202\323\344\223\002\020:\001*\"\013/v1/project'
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._options = None
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._serialized_options = b'\202\323\344\223\002&:\001*\"!/v1/project/{project_id}/add_user'
   _PROJECTSERVICE.methods_by_name['GetProject']._options = None
   _PROJECTSERVICE.methods_by_name['GetProject']._serialized_options = b'\202\323\344\223\002\032\022\030/v1/project/{project_id}'
   _PROJECTSERVICE.methods_by_name['GetProjects']._options = None
@@ -41,51 +41,51 @@
   _PROJECTSERVICE.methods_by_name['GetUserPermissionsForProject']._options = None
   _PROJECTSERVICE.methods_by_name['GetUserPermissionsForProject']._serialized_options = b'\202\323\344\223\002#\022!/v1/project/{project_id}/get_user'
   _PROJECTSERVICE.methods_by_name['GetAllUserPermissionsForProject']._options = None
   _PROJECTSERVICE.methods_by_name['GetAllUserPermissionsForProject']._serialized_options = b'\202\323\344\223\002$\022\"/v1/project/{project_id}/get_users'
   _PROJECTSERVICE.methods_by_name['EditUserPermissionsForProject']._options = None
   _PROJECTSERVICE.methods_by_name['EditUserPermissionsForProject']._serialized_options = b'\202\323\344\223\002\':\001*2\"/v1/project/{project_id}/edit_user'
   _CREATEPROJECTREQUEST._serialized_start=204
-  _CREATEPROJECTREQUEST._serialized_end=280
-  _CREATEPROJECTRESPONSE._serialized_start=282
-  _CREATEPROJECTRESPONSE._serialized_end=336
-  _ADDUSERTOPROJECTREQUEST._serialized_start=339
-  _ADDUSERTOPROJECTREQUEST._serialized_end=484
-  _ADDUSERTOPROJECTRESPONSE._serialized_start=486
-  _ADDUSERTOPROJECTRESPONSE._serialized_end=512
-  _GETPROJECTREQUEST._serialized_start=514
-  _GETPROJECTREQUEST._serialized_end=564
-  _GETPROJECTRESPONSE._serialized_start=566
-  _GETPROJECTRESPONSE._serialized_end=658
-  _GETPROJECTSREQUEST._serialized_start=660
-  _GETPROJECTSREQUEST._serialized_end=680
-  _GETPROJECTSRESPONSE._serialized_start=682
-  _GETPROJECTSRESPONSE._serialized_end=777
-  _DESTROYPROJECTREQUEST._serialized_start=779
-  _DESTROYPROJECTREQUEST._serialized_end=833
-  _DESTROYPROJECTRESPONSE._serialized_start=835
-  _DESTROYPROJECTRESPONSE._serialized_end=859
-  _UPDATEPROJECTREQUEST._serialized_start=861
-  _UPDATEPROJECTREQUEST._serialized_end=968
-  _UPDATEPROJECTRESPONSE._serialized_start=970
-  _UPDATEPROJECTRESPONSE._serialized_end=1065
-  _REMOVEUSERFROMPROJECTREQUEST._serialized_start=1067
-  _REMOVEUSERFROMPROJECTREQUEST._serialized_end=1153
-  _REMOVEUSERFROMPROJECTRESPONSE._serialized_start=1155
-  _REMOVEUSERFROMPROJECTRESPONSE._serialized_end=1186
-  _GETUSERPERMISSIONSFORPROJECTREQUEST._serialized_start=1188
-  _GETUSERPERMISSIONSFORPROJECTREQUEST._serialized_end=1281
-  _GETUSERPERMISSIONSFORPROJECTRESPONSE._serialized_start=1284
-  _GETUSERPERMISSIONSFORPROJECTRESPONSE._serialized_end=1422
-  _EDITUSERPERMISSIONSFORPROJECTREQUEST._serialized_start=1425
-  _EDITUSERPERMISSIONSFORPROJECTREQUEST._serialized_end=1583
-  _EDITUSERPERMISSIONSFORPROJECTRESPONSE._serialized_start=1585
-  _EDITUSERPERMISSIONSFORPROJECTRESPONSE._serialized_end=1624
-  _USERWITHPROJECTPERMISSIONS._serialized_start=1627
-  _USERWITHPROJECTPERMISSIONS._serialized_end=1801
-  _GETALLUSERPERMISSIONSFORPROJECTREQUEST._serialized_start=1803
-  _GETALLUSERPERMISSIONSFORPROJECTREQUEST._serialized_end=1874
-  _GETALLUSERPERMISSIONSFORPROJECTRESPONSE._serialized_start=1876
-  _GETALLUSERPERMISSIONSFORPROJECTRESPONSE._serialized_end=1998
-  _PROJECTSERVICE._serialized_start=2001
-  _PROJECTSERVICE._serialized_end=3809
+  _CREATEPROJECTREQUEST._serialized_end=300
+  _CREATEPROJECTRESPONSE._serialized_start=302
+  _CREATEPROJECTRESPONSE._serialized_end=356
+  _ADDUSERTOPROJECTREQUEST._serialized_start=359
+  _ADDUSERTOPROJECTREQUEST._serialized_end=504
+  _ADDUSERTOPROJECTRESPONSE._serialized_start=506
+  _ADDUSERTOPROJECTRESPONSE._serialized_end=532
+  _GETPROJECTREQUEST._serialized_start=534
+  _GETPROJECTREQUEST._serialized_end=584
+  _GETPROJECTRESPONSE._serialized_start=586
+  _GETPROJECTRESPONSE._serialized_end=678
+  _GETPROJECTSREQUEST._serialized_start=680
+  _GETPROJECTSREQUEST._serialized_end=700
+  _GETPROJECTSRESPONSE._serialized_start=702
+  _GETPROJECTSRESPONSE._serialized_end=797
+  _DESTROYPROJECTREQUEST._serialized_start=799
+  _DESTROYPROJECTREQUEST._serialized_end=853
+  _DESTROYPROJECTRESPONSE._serialized_start=855
+  _DESTROYPROJECTRESPONSE._serialized_end=879
+  _UPDATEPROJECTREQUEST._serialized_start=881
+  _UPDATEPROJECTREQUEST._serialized_end=1008
+  _UPDATEPROJECTRESPONSE._serialized_start=1010
+  _UPDATEPROJECTRESPONSE._serialized_end=1105
+  _REMOVEUSERFROMPROJECTREQUEST._serialized_start=1107
+  _REMOVEUSERFROMPROJECTREQUEST._serialized_end=1193
+  _REMOVEUSERFROMPROJECTRESPONSE._serialized_start=1195
+  _REMOVEUSERFROMPROJECTRESPONSE._serialized_end=1226
+  _GETUSERPERMISSIONSFORPROJECTREQUEST._serialized_start=1228
+  _GETUSERPERMISSIONSFORPROJECTREQUEST._serialized_end=1321
+  _GETUSERPERMISSIONSFORPROJECTRESPONSE._serialized_start=1324
+  _GETUSERPERMISSIONSFORPROJECTRESPONSE._serialized_end=1462
+  _EDITUSERPERMISSIONSFORPROJECTREQUEST._serialized_start=1465
+  _EDITUSERPERMISSIONSFORPROJECTREQUEST._serialized_end=1623
+  _EDITUSERPERMISSIONSFORPROJECTRESPONSE._serialized_start=1625
+  _EDITUSERPERMISSIONSFORPROJECTRESPONSE._serialized_end=1664
+  _USERWITHPROJECTPERMISSIONS._serialized_start=1667
+  _USERWITHPROJECTPERMISSIONS._serialized_end=1841
+  _GETALLUSERPERMISSIONSFORPROJECTREQUEST._serialized_start=1843
+  _GETALLUSERPERMISSIONSFORPROJECTREQUEST._serialized_end=1914
+  _GETALLUSERPERMISSIONSFORPROJECTRESPONSE._serialized_start=1916
+  _GETALLUSERPERMISSIONSFORPROJECTRESPONSE._serialized_end=2038
+  _PROJECTSERVICE._serialized_start=2041
+  _PROJECTSERVICE._serialized_end=3849
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/project_service_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,22 @@
     def __init__(self, project_id: _Optional[str] = ..., user_permission: _Optional[_Union[_auth_pb2.ProjectPermission, _Mapping]] = ...) -> None: ...
 
 class AddUserToProjectResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class CreateProjectRequest(_message.Message):
-    __slots__ = ["description", "name"]
+    __slots__ = ["description", "flag", "name"]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    FLAG_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     description: str
+    flag: int
     name: str
-    def __init__(self, name: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
+    def __init__(self, name: _Optional[str] = ..., description: _Optional[str] = ..., flag: _Optional[int] = ...) -> None: ...
 
 class CreateProjectResponse(_message.Message):
     __slots__ = ["project_id"]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     project_id: str
     def __init__(self, project_id: _Optional[str] = ...) -> None: ...
 
@@ -113,22 +115,24 @@
     def __init__(self, project_id: _Optional[str] = ..., user_id: _Optional[str] = ...) -> None: ...
 
 class RemoveUserFromProjectResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class UpdateProjectRequest(_message.Message):
-    __slots__ = ["description", "name", "project_id"]
+    __slots__ = ["description", "flag", "name", "project_id"]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    FLAG_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     description: str
+    flag: int
     name: str
     project_id: str
-    def __init__(self, project_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
+    def __init__(self, project_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., flag: _Optional[int] = ...) -> None: ...
 
 class UpdateProjectResponse(_message.Message):
     __slots__ = ["project"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
     project: _auth_pb2.ProjectOverview
     def __init__(self, project: _Optional[_Union[_auth_pb2.ProjectOverview, _Mapping]] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/project_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/aruna/api/storage/services/v1/user_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc8/aruna/api/storage/services/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc7/setup.py` & `Aruna-Python-API-1.1.0rc8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='Aruna-Python-API',
-    version="1.1.0-rc.7",
+    version="1.1.0-rc.8",
     description='Aruna Object Storage Python API builds',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ArunaStorage/python-api',
     license='Apache 2.0',
     author='Marius Dieckmann, Jannis Hochmuth',
     author_email='marius.dieckmann@computational.bio.uni-giessen.de, '
```

