# Comparing `tmp/hopsworks-3.2.0rc0.tar.gz` & `tmp/hopsworks-3.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hopsworks-3.2.0rc0.tar", last modified: Wed Apr 12 12:52:06 2023, max compression
+gzip compressed data, was "hopsworks-3.3.0rc0.tar", last modified: Mon Jul  3 12:19:00 2023, max compression
```

## Comparing `hopsworks-3.2.0rc0.tar` & `hopsworks-3.3.0rc0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/
--rw-r--r--   0     1006     1006       40 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/MANIFEST.in
--rw-r--r--   0     1006     1006     3473 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/PKG-INFO
--rw-r--r--   0     1006     1006     2061 2023-04-12 12:52:05.000000 hopsworks-3.2.0rc0/README.md
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.391673 hopsworks-3.2.0rc0/hopsworks/
--rw-r--r--   0     1006     1006    10699 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.395673 hopsworks-3.2.0rc0/hopsworks/client/
--rw-r--r--   0     1006     1006     1552 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/__init__.py
--rw-r--r--   0     1006     1006     1132 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/auth.py
--rw-r--r--   0     1006     1006     6523 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/base.py
--rw-r--r--   0     1006     1006     2308 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/exceptions.py
--rw-r--r--   0     1006     1006     5553 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/external.py
--rw-r--r--   0     1006     1006     8091 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/client/hopsworks.py
--rw-r--r--   0     1006     1006     1493 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/command.py
--rw-r--r--   0     1006     1006    12491 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/connection.py
--rw-r--r--   0     1006     1006     4461 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/constants.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.395673 hopsworks-3.2.0rc0/hopsworks/core/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/__init__.py
--rw-r--r--   0     1006     1006    10113 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/dataset_api.py
--rw-r--r--   0     1006     1006     3639 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/environment_api.py
--rw-r--r--   0     1006     1006     2502 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/execution_api.py
--rw-r--r--   0     1006     1006    15858 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/git_api.py
--rw-r--r--   0     1006     1006     1419 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/git_op_execution_api.py
--rw-r--r--   0     1006     1006     3289 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/git_provider_api.py
--rw-r--r--   0     1006     1006     3673 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/git_remote_api.py
--rw-r--r--   0     1006     1006     5644 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/job_api.py
--rw-r--r--   0     1006     1006    11477 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/kafka_api.py
--rw-r--r--   0     1006     1006     1602 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/library_api.py
--rw-r--r--   0     1006     1006     2984 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/opensearch_api.py
--rw-r--r--   0     1006     1006     3441 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/project_api.py
--rw-r--r--   0     1006     1006     3890 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/secret_api.py
--rw-r--r--   0     1006     1006     1051 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/core/variable_api.py
--rw-r--r--   0     1006     1006     1651 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/decorators.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/hopsworks/engine/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/engine/__init__.py
--rw-r--r--   0     1006     1006     3504 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/engine/environment_engine.py
--rw-r--r--   0     1006     1006     4835 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/engine/execution_engine.py
--rw-r--r--   0     1006     1006     2025 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/engine/git_engine.py
--rw-r--r--   0     1006     1006     4990 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/environment.py
--rw-r--r--   0     1006     1006     6897 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/execution.py
--rw-r--r--   0     1006     1006     2350 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_commit.py
--rw-r--r--   0     1006     1006     2163 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_file_status.py
--rw-r--r--   0     1006     1006     3469 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_op_execution.py
--rw-r--r--   0     1006     1006     2364 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_provider.py
--rw-r--r--   0     1006     1006     2267 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_remote.py
--rw-r--r--   0     1006     1006     8756 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/git_repo.py
--rw-r--r--   0     1006     1006     5909 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/job.py
--rw-r--r--   0     1006     1006     2748 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/kafka_schema.py
--rw-r--r--   0     1006     1006     3310 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/kafka_topic.py
--rw-r--r--   0     1006     1006     1649 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/library.py
--rw-r--r--   0     1006     1006     6451 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/project.py
--rw-r--r--   0     1006     1006     2919 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/secret.py
--rw-r--r--   0     1006     1006     2545 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/user.py
--rw-r--r--   0     1006     1006     2830 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/util.py
--rw-r--r--   0     1006     1006      631 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/hopsworks/version.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.395673 hopsworks-3.2.0rc0/hopsworks.egg-info/
--rw-r--r--   0     1006     1006     3473 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     1566 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      331 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/requires.txt
--rw-r--r--   0     1006     1006       16 2023-04-12 12:52:06.000000 hopsworks-3.2.0rc0/hopsworks.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/setup.cfg
--rw-r--r--   0     1006     1006     1805 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/setup.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/tests/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/tests/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:52:06.399673 hopsworks-3.2.0rc0/tests/hopsworks/
--rw-r--r--   0     1006     1006      605 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/tests/hopsworks/__init__.py
--rw-r--r--   0     1006     1006     7564 2023-04-12 12:52:01.000000 hopsworks-3.2.0rc0/tests/hopsworks/test_login.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:19:00.673378 hopsworks-3.3.0rc0/
+-rw-r--r--   0     1006     1006       40 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/MANIFEST.in
+-rw-r--r--   0     1006     1006     3473 2023-07-03 12:19:00.673378 hopsworks-3.3.0rc0/PKG-INFO
+-rw-r--r--   0     1006     1006     2061 2023-07-03 12:18:58.000000 hopsworks-3.3.0rc0/README.md
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:19:00.665378 hopsworks-3.3.0rc0/hopsworks/
+-rw-r--r--   0     1006     1006    10722 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:19:00.669378 hopsworks-3.3.0rc0/hopsworks/client/
+-rw-r--r--   0     1006     1006     1763 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/client/__init__.py
+-rw-r--r--   0     1006     1006     1132 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/client/auth.py
+-rw-r--r--   0     1006     1006     6523 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/client/base.py
+-rw-r--r--   0     1006     1006     2308 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/client/exceptions.py
+-rw-r--r--   0     1006     1006     5553 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/client/external.py
+-rw-r--r--   0     1006     1006     8091 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/client/hopsworks.py
+-rw-r--r--   0     1006     1006     1493 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/command.py
+-rw-r--r--   0     1006     1006    12731 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/connection.py
+-rw-r--r--   0     1006     1006     4462 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/constants.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:19:00.673378 hopsworks-3.3.0rc0/hopsworks/core/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/__init__.py
+-rw-r--r--   0     1006     1006    10113 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/dataset_api.py
+-rw-r--r--   0     1006     1006     3795 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/core/environment_api.py
+-rw-r--r--   0     1006     1006     2502 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/execution_api.py
+-rw-r--r--   0     1006     1006    15858 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/git_api.py
+-rw-r--r--   0     1006     1006     1419 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/git_op_execution_api.py
+-rw-r--r--   0     1006     1006     3289 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/git_provider_api.py
+-rw-r--r--   0     1006     1006     3673 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/git_remote_api.py
+-rw-r--r--   0     1006     1006     5644 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/job_api.py
+-rw-r--r--   0     1006     1006    11477 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/kafka_api.py
+-rw-r--r--   0     1006     1006     1588 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/core/library_api.py
+-rw-r--r--   0     1006     1006     2984 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/opensearch_api.py
+-rw-r--r--   0     1006     1006     3441 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/project_api.py
+-rw-r--r--   0     1006     1006     3890 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/core/secret_api.py
+-rw-r--r--   0     1006     1006     1337 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/core/variable_api.py
+-rw-r--r--   0     1006     1006     1651 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/decorators.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:19:00.673378 hopsworks-3.3.0rc0/hopsworks/engine/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/engine/__init__.py
+-rw-r--r--   0     1006     1006     3471 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/engine/environment_engine.py
+-rw-r--r--   0     1006     1006     4835 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/engine/execution_engine.py
+-rw-r--r--   0     1006     1006     2025 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/engine/git_engine.py
+-rw-r--r--   0     1006     1006     5670 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/environment.py
+-rw-r--r--   0     1006     1006     6897 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/execution.py
+-rw-r--r--   0     1006     1006     2350 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/git_commit.py
+-rw-r--r--   0     1006     1006     2163 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/git_file_status.py
+-rw-r--r--   0     1006     1006     3469 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/git_op_execution.py
+-rw-r--r--   0     1006     1006     2364 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/git_provider.py
+-rw-r--r--   0     1006     1006     2267 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/git_remote.py
+-rw-r--r--   0     1006     1006     8756 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/git_repo.py
+-rw-r--r--   0     1006     1006     5909 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/job.py
+-rw-r--r--   0     1006     1006     2748 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/kafka_schema.py
+-rw-r--r--   0     1006     1006     3310 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/kafka_topic.py
+-rw-r--r--   0     1006     1006     1649 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/library.py
+-rw-r--r--   0     1006     1006     6578 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/project.py
+-rw-r--r--   0     1006     1006     2919 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/secret.py
+-rw-r--r--   0     1006     1006     2545 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/user.py
+-rw-r--r--   0     1006     1006     2830 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/hopsworks/util.py
+-rw-r--r--   0     1006     1006      631 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/hopsworks/version.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:19:00.665378 hopsworks-3.3.0rc0/hopsworks.egg-info/
+-rw-r--r--   0     1006     1006     3473 2023-07-03 12:19:00.000000 hopsworks-3.3.0rc0/hopsworks.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     1566 2023-07-03 12:19:00.000000 hopsworks-3.3.0rc0/hopsworks.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-07-03 12:19:00.000000 hopsworks-3.3.0rc0/hopsworks.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      504 2023-07-03 12:19:00.000000 hopsworks-3.3.0rc0/hopsworks.egg-info/requires.txt
+-rw-r--r--   0     1006     1006       16 2023-07-03 12:19:00.000000 hopsworks-3.3.0rc0/hopsworks.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-07-03 12:19:00.673378 hopsworks-3.3.0rc0/setup.cfg
+-rw-r--r--   0     1006     1006     1980 2023-07-03 12:18:49.000000 hopsworks-3.3.0rc0/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:19:00.673378 hopsworks-3.3.0rc0/tests/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/tests/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-07-03 12:19:00.673378 hopsworks-3.3.0rc0/tests/hopsworks/
+-rw-r--r--   0     1006     1006      605 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/tests/hopsworks/__init__.py
+-rw-r--r--   0     1006     1006     7564 2023-06-27 14:52:13.000000 hopsworks-3.3.0rc0/tests/hopsworks/test_login.py
```

### Comparing `hopsworks-3.2.0rc0/PKG-INFO` & `hopsworks-3.3.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hopsworks
-Version: 3.2.0rc0
+Version: 3.3.0rc0
 Summary: HOPSWORKS: An environment independent client to interact with the Hopsworks API
 Home-page: https://github.com/logicalclocks/hopsworks-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.2.0rc0
+Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.3.0rc0
 Description: # Hopsworks Client
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hopsworks Version: 3.2.0rc0 Summary: HOPSWORKS: An
+Metadata-Version: 2.1 Name: hopsworks Version: 3.3.0rc0 Summary: HOPSWORKS: An
 environment independent client to interact with the Hopsworks API Home-page:
 https://github.com/logicalclocks/hopsworks-api Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/hopsworks-api/releases/tag/3.2.0rc0
+https://github.com/logicalclocks/hopsworks-api/releases/tag/3.3.0rc0
 Description: # Hopsworks Client
    [Hopsworks_Community] [Hopsworks_Documentation] [PyPiStatus] [Downloads]
                              [CodeStyle] [License]
 *hopsworks* is the python API for interacting with a Hopsworks cluster. ##
 Getting Started On Hopsworks Instantiate a connection and get the project
 object ```python import hopsworks connection = hopsworks.connection() project =
 connection.get_project("my_project") ``` Create a new project ```python project
```

### Comparing `hopsworks-3.2.0rc0/README.md` & `hopsworks-3.3.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/__init__.py` & `hopsworks-3.3.0rc0/hopsworks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 import sys
 import getpass
 import tempfile
 from pathlib import Path
 
 from hopsworks.client.exceptions import RestAPIError, ProjectException
-from hopsworks import version
+from hopsworks import version, constants
 from hopsworks.connection import Connection
 
 # Needs to run before import of hsml and hsfs
 warnings.filterwarnings(action="ignore", category=UserWarning, module=r".*psycopg2")
 
 import hsml  # noqa: F401, E402
 import hsfs  # noqa: F401, E402
@@ -131,15 +131,15 @@
     if project is None and "HOPSWORKS_PROJECT" in os.environ:
         project = os.environ["HOPSWORKS_PROJECT"]
 
     # If host argument not defined, get HOPSWORKS_HOST environment variable
     if host is None and "HOPSWORKS_HOST" in os.environ:
         host = os.environ["HOPSWORKS_HOST"]
     elif host is None:  # Always do a fallback to Serverless Hopsworks if not defined
-        host = "c.app.hopsworks.ai"
+        host = constants.HOSTS.APP_HOST
 
     # If port same as default, get HOPSWORKS_HOST environment variable
     if port == 443 and "HOPSWORKS_PORT" in os.environ:
         port = os.environ["HOPSWORKS_PORT"]
 
     # This .hw_api_key is created when a user logs into Serverless Hopsworks the first time.
     # It is then used only for future login calls to Serverless. For other Hopsworks installations it's ignored.
@@ -159,15 +159,15 @@
             finally:
                 file.close()
         else:
             raise IOError(
                 "Could not find api key file on path: {}".format(api_key_file)
             )
     # If user connected to Serverless Hopsworks, and the cached .hw_api_key exists, then use it.
-    elif os.path.exists(api_key_path) and host == "c.app.hopsworks.ai":
+    elif os.path.exists(api_key_path) and host == constants.HOSTS.APP_HOST:
         try:
             _hw_connection = _hw_connection(
                 host=host, port=port, api_key_file=api_key_path
             )
             _connected_project = _prompt_project(_hw_connection, project)
             print(
                 "\nLogged in to project, explore it here "
@@ -175,15 +175,15 @@
             )
             return _connected_project
         except RestAPIError:
             logout()
             # API Key may be invalid, have the user supply it again
             os.remove(api_key_path)
 
-    if api_key is None and host == "c.app.hopsworks.ai":
+    if api_key is None and host == constants.HOSTS.APP_HOST:
         print(
             "Copy your Api Key (first register/login): https://c.app.hopsworks.ai/account/api/generated"
         )
         api_key = getpass.getpass(prompt="\nPaste it here: ")
 
         # If api key was provided as input, save the API key locally on disk to avoid users having to enter it again in the same environment
         Path(os.path.dirname(api_key_path)).mkdir(parents=True, exist_ok=True)
```

### Comparing `hopsworks-3.2.0rc0/hopsworks/client/__init__.py` & `hopsworks-3.3.0rc0/hopsworks/client/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 from hopsworks.client import external, hopsworks
 
 _client = None
+_python_version = None
 
 
 def init(
     client_type,
     host=None,
     port=None,
     project=None,
@@ -50,11 +51,21 @@
 def get_instance():
     global _client
     if _client:
         return _client
     raise Exception("Couldn't find client. Try reconnecting to Hopsworks.")
 
 
+def get_python_version():
+    global _python_version
+    return _python_version
+
+
+def set_python_version(python_version):
+    global _python_version
+    _python_version = python_version
+
+
 def stop():
     global _client
     _client._close()
     _client = None
```

### Comparing `hopsworks-3.2.0rc0/hopsworks/client/auth.py` & `hopsworks-3.3.0rc0/hopsworks/client/auth.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/client/base.py` & `hopsworks-3.3.0rc0/hopsworks/client/base.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/client/exceptions.py` & `hopsworks-3.3.0rc0/hopsworks/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/client/external.py` & `hopsworks-3.3.0rc0/hopsworks/client/external.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/client/hopsworks.py` & `hopsworks-3.3.0rc0/hopsworks/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/command.py` & `hopsworks-3.3.0rc0/hopsworks/command.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/connection.py` & `hopsworks-3.3.0rc0/hopsworks/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,20 @@
             warnings.warn(
                 "The installed hopsworks client version {0} may not be compatible with the connected Hopsworks backend version {1}. \nTo ensure compatibility please install the latest bug fix release matching the minor version of your backend ({2}) by running 'pip install hopsworks=={2}.*'".format(
                     client_version, backend_version, major_minor_backend
                 )
             )
             sys.stderr.flush()
 
+    def _set_client_variables(self):
+        python_version = self._variable_api.get_variable(
+            "docker_base_image_python_version"
+        )
+        client.set_python_version(python_version)
+
     @not_connected
     def connect(self):
         """Instantiate the connection.
 
         Creating a `Connection` object implicitly calls this method for you to
         instantiate the connection. However, it is possible to close the connection
         gracefully with the `close()` method, in order to clean up materialized
@@ -256,14 +262,15 @@
             raise
         print(
             "Connected. Call `.close()` to terminate connection gracefully.",
             flush=True,
         )
 
         self._check_compatibility()
+        self._set_client_variables()
 
     def close(self):
         """Close a connection gracefully.
 
         This will clean up any materialized certificates on the local file system of
         external environments such as AWS SageMaker.
```

### Comparing `hopsworks-3.2.0rc0/hopsworks/constants.py` & `hopsworks-3.3.0rc0/hopsworks/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,9 +129,9 @@
     PEM_CA_CHAIN_CERTIFICATE_CONFIG = "ca_chain.pem"
     DOMAIN_CA_TRUSTSTORE = "domain_ca_truststore"
     CRYPTO_MATERIAL_PASSWORD = "material_passwd"
     PEM_CA_ROOT_CERT = "/srv/hops/kagent/host-certs/hops_root_ca.pem"
     SSL_ENABLED = "ipc.server.ssl.enabled"
 
 
-class PYTHON_CONFIG:
-    PYTHON_VERSION = "3.8"
+class HOSTS:
+    APP_HOST = "c.app.hopsworks.ai"
```

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/__init__.py` & `hopsworks-3.3.0rc0/hopsworks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/dataset_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/environment_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/environment_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-from hopsworks import client, environment, constants
+from hopsworks import client, environment
 from hopsworks.engine import environment_engine
 
 
 class EnvironmentApi:
     def __init__(
         self,
         project_id,
@@ -53,28 +53,45 @@
         _client = client.get_instance()
 
         path_params = [
             "project",
             self._project_id,
             "python",
             "environments",
-            constants.PYTHON_CONFIG.PYTHON_VERSION,
+            client.get_python_version(),
         ]
         headers = {"content-type": "application/json"}
         env = environment.Environment.from_response_json(
             _client._send_request("POST", path_params, headers=headers),
             self._project_id,
             self._project_name,
         )
 
         if await_creation:
             self._environment_engine.await_environment_command()
 
         return env
 
+    def _get_environments(self):
+        """
+        Get all available python environments in the project
+        """
+        _client = client.get_instance()
+
+        path_params = ["project", self._project_id, "python", "environments"]
+        query_params = {"expand": ["libraries", "commands"]}
+        headers = {"content-type": "application/json"}
+        return environment.Environment.from_response_json(
+            _client._send_request(
+                "GET", path_params, query_params=query_params, headers=headers
+            ),
+            self._project_id,
+            self._project_name,
+        )
+
     def get_environment(self):
         """Get handle for the Python environment for the project
 
         ```python
 
         import hopsworks
 
@@ -86,39 +103,26 @@
 
         ```
         # Returns
             `Environment`: The Environment object
         # Raises
             `RestAPIError`: If unable to get the environment
         """
-        _client = client.get_instance()
-
-        path_params = [
-            "project",
-            self._project_id,
-            "python",
-            "environments",
-            constants.PYTHON_CONFIG.PYTHON_VERSION,
-        ]
-        query_params = {"expand": ["libraries", "commands"]}
-        headers = {"content-type": "application/json"}
-        return environment.Environment.from_response_json(
-            _client._send_request(
-                "GET", path_params, query_params=query_params, headers=headers
-            ),
-            self._project_id,
-            self._project_name,
-        )
+        project_envs = self._get_environments()
+        if len(project_envs) == 0:
+            return None
+        elif len(project_envs) > 0:
+            return project_envs[0]
 
-    def _delete(self):
+    def _delete(self, python_version):
         """Delete the project Python environment"""
         _client = client.get_instance()
 
         path_params = [
             "project",
             self._project_id,
             "python",
             "environments",
-            constants.PYTHON_CONFIG.PYTHON_VERSION,
+            python_version,
         ]
         headers = {"content-type": "application/json"}
         _client._send_request("DELETE", path_params, headers=headers),
```

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/execution_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/execution_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/git_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/git_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/git_op_execution_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/git_op_execution_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/git_provider_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/git_provider_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/git_remote_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/git_remote_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/job_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/kafka_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/library_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/library_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 import json
 
-from hopsworks import client, library, constants
+from hopsworks import client, library
 
 
 class LibraryApi:
     def __init__(
         self,
         project_id,
         project_name,
     ):
         self._project_id = project_id
         self._project_name = project_name
 
-    def install(self, library_name: str, library_spec: dict):
+    def install(self, library_name: str, python_version: str, library_spec: dict):
         """Create Python environment for the project"""
         _client = client.get_instance()
 
         path_params = [
             "project",
             self._project_id,
             "python",
             "environments",
-            constants.PYTHON_CONFIG.PYTHON_VERSION,
+            python_version,
             "libraries",
             library_name,
         ]
 
         headers = {"content-type": "application/json"}
         library_rest = library.Library.from_response_json(
             _client._send_request(
```

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/opensearch_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/opensearch_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/project_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/core/secret_api.py` & `hopsworks-3.3.0rc0/hopsworks/core/secret_api.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/decorators.py` & `hopsworks-3.3.0rc0/hopsworks/decorators.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/engine/__init__.py` & `hopsworks-3.3.0rc0/hopsworks/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/engine/environment_engine.py` & `hopsworks-3.3.0rc0/hopsworks/engine/environment_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 import time
 
-from hopsworks import client, library, environment, command, constants
+from hopsworks import client, library, environment, command
 from hopsworks.client.exceptions import RestAPIError, EnvironmentException
 
 
 class EnvironmentEngine:
     def __init__(self, project_id):
         self._project_id = project_id
 
@@ -58,15 +58,15 @@
         _client = client.get_instance()
 
         path_params = [
             "project",
             self._project_id,
             "python",
             "environments",
-            constants.PYTHON_CONFIG.PYTHON_VERSION,
+            client.get_python_version(),
             "libraries",
             library_name,
         ]
 
         query_params = {"expand": "commands"}
         headers = {"content-type": "application/json"}
 
@@ -89,15 +89,15 @@
         _client = client.get_instance()
 
         path_params = [
             "project",
             self._project_id,
             "python",
             "environments",
-            constants.PYTHON_CONFIG.PYTHON_VERSION,
+            client.get_python_version(),
         ]
 
         query_params = {"expand": "commands"}
         headers = {"content-type": "application/json"}
 
         return environment.Environment.from_response_json(
             _client._send_request(
```

### Comparing `hopsworks-3.2.0rc0/hopsworks/engine/execution_engine.py` & `hopsworks-3.3.0rc0/hopsworks/engine/execution_engine.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/engine/git_engine.py` & `hopsworks-3.3.0rc0/hopsworks/engine/git_engine.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/environment.py` & `hopsworks-3.3.0rc0/hopsworks/environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,15 +51,34 @@
         self._environment_engine = environment_engine.EnvironmentEngine(project_id)
         self._library_api = library_api.LibraryApi(project_id, project_name)
         self._environment_api = environment_api.EnvironmentApi(project_id, project_name)
 
     @classmethod
     def from_response_json(cls, json_dict, project_id, project_name):
         json_decamelized = humps.decamelize(json_dict)
-        return cls(**json_decamelized, project_id=project_id, project_name=project_name)
+        if "count" in json_decamelized:
+            return [
+                cls(
+                    **env,
+                    project_id=project_id,
+                    project_name=project_name,
+                )
+                for env in json_decamelized["items"]
+            ]
+        else:
+            return cls(
+                **json_decamelized,
+                project_id=project_id,
+                project_name=project_name,
+            )
+
+    @property
+    def python_version(self):
+        """Python version of the environment"""
+        return self._python_version
 
     def install_wheel(self, path, await_installation=True):
         """Install a python library packaged in a wheel file
 
         ```python
 
         import hopsworks
@@ -91,15 +110,17 @@
 
         library_spec = {
             "dependencyUrl": path,
             "channelUrl": "wheel",
             "packageSource": "WHEEL",
         }
 
-        library_rest = self._library_api.install(library_name, library_spec)
+        library_rest = self._library_api.install(
+            library_name, self.python_version, library_spec
+        )
 
         if await_installation:
             return self._environment_engine.await_library_command(library_name)
 
         return library_rest
 
     def install_requirements(self, path, await_installation=True):
@@ -136,22 +157,27 @@
 
         library_spec = {
             "dependencyUrl": path,
             "channelUrl": "requirements_txt",
             "packageSource": "REQUIREMENTS_TXT",
         }
 
-        library_rest = self._library_api.install(library_name, library_spec)
+        library_rest = self._library_api.install(
+            library_name, self.python_version, library_spec
+        )
 
         if await_installation:
             return self._environment_engine.await_library_command(library_name)
 
         return library_rest
 
     def delete(self):
         """Delete the environment
         !!! danger "Potentially dangerous operation"
             This operation deletes the python environment.
         # Raises
             `RestAPIError`.
         """
-        self._environment_api._delete()
+        self._environment_api._delete(self.python_version)
+
+    def __repr__(self):
+        return f"Environment({self._python_version!r})"
```

### Comparing `hopsworks-3.2.0rc0/hopsworks/execution.py` & `hopsworks-3.3.0rc0/hopsworks/execution.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/git_commit.py` & `hopsworks-3.3.0rc0/hopsworks/git_commit.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/git_file_status.py` & `hopsworks-3.3.0rc0/hopsworks/git_file_status.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/git_op_execution.py` & `hopsworks-3.3.0rc0/hopsworks/git_op_execution.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/git_provider.py` & `hopsworks-3.3.0rc0/hopsworks/git_provider.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/git_remote.py` & `hopsworks-3.3.0rc0/hopsworks/git_remote.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/git_repo.py` & `hopsworks-3.3.0rc0/hopsworks/git_repo.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/job.py` & `hopsworks-3.3.0rc0/hopsworks/job.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/kafka_schema.py` & `hopsworks-3.3.0rc0/hopsworks/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/kafka_topic.py` & `hopsworks-3.3.0rc0/hopsworks/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/library.py` & `hopsworks-3.3.0rc0/hopsworks/library.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/project.py` & `hopsworks-3.3.0rc0/hopsworks/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 import humps
 import json
 
-from hopsworks import util, client
+from hopsworks import util, client, constants
 from hopsworks.client.external import Client
 from hopsworks.core import (
     job_api,
     git_api,
     dataset_api,
     kafka_api,
     opensearch_api,
@@ -104,20 +104,23 @@
         # Raises
             `RestAPIError`: If unable to connect
         """
         from hsfs import connection
 
         _client = client.get_instance()
         if type(_client) == Client:  # If external client
+            engine = None
+            if _client._host == constants.HOSTS.APP_HOST:
+                engine = "python"
             return connection(
                 host=_client._host,
                 port=_client._port,
                 project=self.name,
                 api_key_value=_client._auth._token,
-                engine="python",
+                engine=engine,
             ).get_feature_store()
         else:
             return connection().get_feature_store()  # If internal client
 
     def get_model_registry(self):
         """Connect to Project's Model Registry API.
         # Returns
```

### Comparing `hopsworks-3.2.0rc0/hopsworks/secret.py` & `hopsworks-3.3.0rc0/hopsworks/secret.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/user.py` & `hopsworks-3.3.0rc0/hopsworks/user.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/util.py` & `hopsworks-3.3.0rc0/hopsworks/util.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/hopsworks/version.py` & `hopsworks-3.3.0rc0/hopsworks/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.2.0rc0"
+__version__ = "3.3.0rc0"
```

### Comparing `hopsworks-3.2.0rc0/hopsworks.egg-info/PKG-INFO` & `hopsworks-3.3.0rc0/hopsworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hopsworks
-Version: 3.2.0rc0
+Version: 3.3.0rc0
 Summary: HOPSWORKS: An environment independent client to interact with the Hopsworks API
 Home-page: https://github.com/logicalclocks/hopsworks-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.2.0rc0
+Download-URL: https://github.com/logicalclocks/hopsworks-api/releases/tag/3.3.0rc0
 Description: # Hopsworks Client
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hopsworks Version: 3.2.0rc0 Summary: HOPSWORKS: An
+Metadata-Version: 2.1 Name: hopsworks Version: 3.3.0rc0 Summary: HOPSWORKS: An
 environment independent client to interact with the Hopsworks API Home-page:
 https://github.com/logicalclocks/hopsworks-api Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/hopsworks-api/releases/tag/3.2.0rc0
+https://github.com/logicalclocks/hopsworks-api/releases/tag/3.3.0rc0
 Description: # Hopsworks Client
    [Hopsworks_Community] [Hopsworks_Documentation] [PyPiStatus] [Downloads]
                              [CodeStyle] [License]
 *hopsworks* is the python API for interacting with a Hopsworks cluster. ##
 Getting Started On Hopsworks Instantiate a connection and get the project
 object ```python import hopsworks connection = hopsworks.connection() project =
 connection.get_project("my_project") ``` Create a new project ```python project
```

### Comparing `hopsworks-3.2.0rc0/hopsworks.egg-info/SOURCES.txt` & `hopsworks-3.3.0rc0/hopsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/setup.py` & `hopsworks-3.3.0rc0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="hopsworks",
     version=__version__,
     install_requires=[
-        "hsfs[python]~=3.2.0rc0",
-        "hsml~=3.2.0rc0",
+        "hsfs @ git+https://git@github.com/logicalclocks/feature-store-api@master#egg=hsfs[python]&subdirectory=python",
+        "hsml @ git+https://git@github.com/logicalclocks/machine-learning-api@main#egg=hsml&subdirectory=python",
         "pyhumps==1.6.1",
         "requests",
         "furl",
         "boto3",
         "pyjks",
         "mock",
         "tqdm",
```

### Comparing `hopsworks-3.2.0rc0/tests/__init__.py` & `hopsworks-3.3.0rc0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/tests/hopsworks/__init__.py` & `hopsworks-3.3.0rc0/tests/hopsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `hopsworks-3.2.0rc0/tests/hopsworks/test_login.py` & `hopsworks-3.3.0rc0/tests/hopsworks/test_login.py`

 * *Files identical despite different names*

