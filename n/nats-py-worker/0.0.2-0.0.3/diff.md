# Comparing `tmp/nats-py-worker-0.0.2.tar.gz` & `tmp/nats-py-worker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats-py-worker-0.0.2.tar", last modified: Fri Jun 30 06:09:41 2023, max compression
+gzip compressed data, was "nats-py-worker-0.0.3.tar", last modified: Mon Jul  3 02:46:47 2023, max compression
```

## Comparing `nats-py-worker-0.0.2.tar` & `nats-py-worker-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:09:41.045691 nats-py-worker-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-30 06:09:28.000000 nats-py-worker-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3613 2023-06-30 06:09:41.045691 nats-py-worker-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-30 06:09:28.000000 nats-py-worker-0.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      993 2023-06-30 06:09:28.000000 nats-py-worker-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 06:09:41.045691 nats-py-worker-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:09:41.042691 nats-py-worker-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:09:41.044691 nats-py-worker-0.0.2/src/nats_py_worker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3613 2023-06-30 06:09:41.000000 nats-py-worker-0.0.2/src/nats_py_worker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-30 06:09:41.000000 nats-py-worker-0.0.2/src/nats_py_worker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 06:09:41.000000 nats-py-worker-0.0.2/src/nats_py_worker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-30 06:09:41.000000 nats-py-worker-0.0.2/src/nats_py_worker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-30 06:09:41.000000 nats-py-worker-0.0.2/src/nats_py_worker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:09:41.044691 nats-py-worker-0.0.2/src/nats_worker/
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-30 06:09:28.000000 nats-py-worker-0.0.2/src/nats_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21592 2023-06-30 06:09:28.000000 nats-py-worker-0.0.2/src/nats_worker/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 06:09:41.044691 nats-py-worker-0.0.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-30 06:09:28.000000 nats-py-worker-0.0.2/tests/test_nats_worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.060284 nats-py-worker-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-03 02:46:47.060284 nats-py-worker-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      993 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 02:46:47.060284 nats-py-worker-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.058283 nats-py-worker-0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.059284 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-03 02:46:47.000000 nats-py-worker-0.0.3/src/nats_py_worker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.059284 nats-py-worker-0.0.3/src/nats_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/src/nats_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21798 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/src/nats_worker/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 02:46:47.060284 nats-py-worker-0.0.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-07-03 02:46:35.000000 nats-py-worker-0.0.3/tests/test_nats_worker.py
```

### Comparing `nats-py-worker-0.0.2/LICENSE` & `nats-py-worker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nats-py-worker-0.0.2/PKG-INFO` & `nats-py-worker-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nats-py-worker
-Version: 0.0.2
+Version: 0.0.3
 Summary: An opinionated utility for using NATS as a worker queue with NATS.py
 License: Copyright (c) 2023 The University of Adelaide
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `nats-py-worker-0.0.2/README.md` & `nats-py-worker-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nats-py-worker-0.0.2/pyproject.toml` & `nats-py-worker-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nats-py-worker-0.0.2/src/nats_py_worker.egg-info/PKG-INFO` & `nats-py-worker-0.0.3/src/nats_py_worker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nats-py-worker
-Version: 0.0.2
+Version: 0.0.3
 Summary: An opinionated utility for using NATS as a worker queue with NATS.py
 License: Copyright (c) 2023 The University of Adelaide
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `nats-py-worker-0.0.2/src/nats_worker/core.py` & `nats-py-worker-0.0.3/src/nats_worker/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,14 +451,18 @@
                     ack_wait=ack_wait,
                     max_ack_pending=1,
                 ):
                     key = key_map(msg)
                     state_entry = await get_value(
                         connection=connection, bucket=bucket, key=key
                     )
+                    if state_entry is None:
+                        state_entry = NatsKeyValue.Entry(
+                            bucket=bucket, key=key, revision=None, value=None
+                        )
                     new_state = await f(state_entry, msg, **kwargs)
                     if new_state is not None:
                         await save_value(
                             connection=connection,
                             bucket=bucket,
                             key=key,
                             value=new_state,
```

### Comparing `nats-py-worker-0.0.2/tests/test_nats_worker.py` & `nats-py-worker-0.0.3/tests/test_nats_worker.py`

 * *Files identical despite different names*

