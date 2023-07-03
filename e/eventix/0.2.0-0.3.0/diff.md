# Comparing `tmp/eventix-0.2.0.tar.gz` & `tmp/eventix-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventix-0.2.0.tar", max compression
+gzip compressed data, was "eventix-0.3.0.tar", max compression
```

## Comparing `eventix-0.2.0.tar` & `eventix-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      103 2023-07-03 12:21:14.593891 eventix-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-10 06:41:07.956006 eventix-0.2.0/eventix/__init__.py
--rw-r--r--   0        0        0      915 2023-07-03 08:40:22.393606 eventix-0.2.0/eventix/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 06:41:07.956006 eventix-0.2.0/eventix/functions/__init__.py
--rw-r--r--   0        0        0     3209 2023-07-03 12:21:07.053990 eventix-0.2.0/eventix/functions/core.py
--rw-r--r--   0        0        0      910 2023-06-28 11:22:43.094568 eventix-0.2.0/eventix/functions/eventflow_client.py
--rw-r--r--   0        0        0     2552 2023-06-20 16:04:58.874051 eventix-0.2.0/eventix/functions/fastapi.py
--rw-r--r--   0        0        0     6082 2023-07-03 12:21:07.085990 eventix-0.2.0/eventix/functions/task.py
--rw-r--r--   0        0        0     1082 2023-07-03 12:21:07.089990 eventix-0.2.0/eventix/functions/task_scheduler.py
--rw-r--r--   0        0        0     3883 2023-07-03 12:21:07.077990 eventix-0.2.0/eventix/functions/task_worker.py
--rw-r--r--   0        0        0      322 2023-06-28 08:36:07.948516 eventix-0.2.0/eventix/functions/tools.py
--rw-r--r--   0        0        0        0 2023-05-10 06:41:07.956006 eventix-0.2.0/eventix/pydantic/__init__.py
--rw-r--r--   0        0        0      380 2023-06-16 15:12:43.406599 eventix-0.2.0/eventix/pydantic/event.py
--rw-r--r--   0        0        0     1951 2023-06-30 12:56:02.843436 eventix-0.2.0/eventix/pydantic/task.py
--rw-r--r--   0        0        0        0 2023-05-10 06:41:07.956006 eventix-0.2.0/eventix/router/__init__.py
--rw-r--r--   0        0        0      517 2023-07-03 12:21:07.089990 eventix-0.2.0/eventix/router/event.py
--rw-r--r--   0        0        0      236 2023-07-03 12:21:07.093990 eventix-0.2.0/eventix/router/metrics.py
--rw-r--r--   0        0        0     1201 2023-07-03 12:21:07.081990 eventix-0.2.0/eventix/router/task.py
--rw-r--r--   0        0        0      958 2023-07-03 12:21:07.065990 eventix-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 eventix-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      103 2023-07-03 12:25:39.726933 eventix-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/__init__.py
+-rw-r--r--   0        0        0      915 2023-07-03 12:32:53.419527 eventix-0.3.0/eventix/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/functions/__init__.py
+-rw-r--r--   0        0        0     3104 2023-07-03 12:35:26.922564 eventix-0.3.0/eventix/functions/core.py
+-rw-r--r--   0        0        0      709 2023-07-03 12:35:26.910564 eventix-0.3.0/eventix/functions/errors.py
+-rw-r--r--   0        0        0      900 2023-07-03 12:36:13.218289 eventix-0.3.0/eventix/functions/eventix_client.py
+-rw-r--r--   0        0        0     2552 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/functions/fastapi.py
+-rw-r--r--   0        0        0     6082 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/functions/task.py
+-rw-r--r--   0        0        0      990 2023-07-03 12:36:06.494329 eventix-0.3.0/eventix/functions/task_scheduler.py
+-rw-r--r--   0        0        0     3879 2023-07-03 12:37:58.589687 eventix-0.3.0/eventix/functions/task_worker.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/functions/tools.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/pydantic/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/pydantic/event.py
+-rw-r--r--   0        0        0     1951 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/pydantic/task.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/router/__init__.py
+-rw-r--r--   0        0        0      517 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/router/event.py
+-rw-r--r--   0        0        0      236 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/router/metrics.py
+-rw-r--r--   0        0        0     1201 2023-07-03 12:25:39.726933 eventix-0.3.0/eventix/router/task.py
+-rw-r--r--   0        0        0      958 2023-07-03 12:39:18.805247 eventix-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 eventix-0.3.0/PKG-INFO
```

### Comparing `eventix-0.2.0/eventix/exceptions/__init__.py` & `eventix-0.3.0/eventix/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `eventix-0.2.0/eventix/functions/core.py` & `eventix-0.3.0/eventix/functions/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import contextlib
 import contextvars
 import functools
 import logging
 import os
-from typing import Callable, Any
+from typing import Callable
 
-from eventix.exceptions import TaskNotUnique
 from eventix.functions.task_scheduler import TaskScheduler
 from eventix.pydantic.task import TaskModel
-from pydantic_db_backend.exceptions import AlreadyExists
 
 log = logging.getLogger(__name__)
 
 
 class EventflowTaskBase(object):
     pass
 
@@ -99,7 +97,9 @@
                     params |= dict(unique_key=unique_key)
 
                 return TaskModel.parse_obj(params)
 
         return EventflowTask()
 
     return inner
+
+
```

### Comparing `eventix-0.2.0/eventix/functions/eventflow_client.py` & `eventix-0.3.0/eventix/functions/eventix_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from requests import Session, Response
 
 import logging
 
 log = logging.getLogger(__name__)
 
 
-class EventflowClientSession(Session):
+class EventixClientSession(Session):
     def __init__(self, base_url: str = None) -> None:
         self.base_url = base_url
         super().__init__()
 
     def request(
         self,
         method: str | bytes,
@@ -23,16 +23,16 @@
             method,
             f"{self.base_url}{url}",
             *args,
             **kwargs
         )
 
 
-class EventflowClient:
-    interface: Any | None = EventflowClientSession()
+class EventixClient:
+    interface: Any | None = EventixClientSession()
     namespace: str | None = None
 
     @classmethod
     def set_base_url(cls, base_url):
-        if isinstance(cls.interface, EventflowClientSession):
-            log.info(f"Setting EventflowClient base_url: {base_url}")
+        if isinstance(cls.interface, EventixClientSession):
+            log.info(f"Setting EventixClient base_url: {base_url}")
             cls.interface.base_url = base_url
```

### Comparing `eventix-0.2.0/eventix/functions/fastapi.py` & `eventix-0.3.0/eventix/functions/fastapi.py`

 * *Files identical despite different names*

### Comparing `eventix-0.2.0/eventix/functions/task.py` & `eventix-0.3.0/eventix/functions/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.2.0/eventix/functions/task_scheduler.py` & `eventix-0.3.0/eventix/functions/task_scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 
 from eventix.exceptions import backend_exceptions
-from eventix.functions.eventflow_client import EventflowClient
+from eventix.functions.errors import raise_errors
+from eventix.functions.eventix_client import EventixClient
 from eventix.pydantic.task import TaskModel
-from pydantic_db_backend.exceptions import AlreadyExists, NotFound, RevisionConflict
-from webexception.webexception import raise_errors
 
 log = logging.getLogger(__name__)
 
 
-class TaskScheduler(EventflowClient):
+class TaskScheduler(EventixClient):
 
     @classmethod
     def schedule(cls, task: TaskModel) -> TaskModel:
         log.debug(f"scheduling task: {task.task} uid: {task.uid} eta: {task.eta} unique_key: {task.unique_key}")
         task.namespace = cls.namespace
         return cls.task_post(task)
```

### Comparing `eventix-0.2.0/eventix/functions/task_worker.py` & `eventix-0.3.0/eventix/functions/task_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import importlib
 import logging
 import time
 from typing import List
 
+from pydantic_db_backend.utils import utcnow
+
 from eventix.exceptions import TaskNotRegistered, backend_exceptions
 from eventix.functions.core import EventflowTaskBase, namespace_context, worker_id_context
-from eventix.functions.eventflow_client import EventflowClient
+from eventix.functions.errors import raise_errors
+from eventix.functions.eventix_client import EventixClient
 from eventix.functions.task import task_set_error
 from eventix.pydantic.task import TaskModel
-from pydantic_db_backend.utils import utcnow
-from webexception.webexception import raise_errors
 
 log = logging.getLogger(__name__)
 
 
-class TaskWorker(EventflowClient):
+class TaskWorker(EventixClient):
     _wait_interval = 10
     _tasks = {}
 
     @classmethod
     def register_tasks(cls, paths=List[str]):
         log.info("registering tasks...")
         # noinspection PyTypeChecker
@@ -105,13 +106,13 @@
 
             with raise_errors(r, backend_exceptions):
                 if r.status_code == 200:
                     tm = TaskModel.parse_raw(r.content)
                     return tm
 
         except Exception as e:
-            log.error("Exception happend calling eventflow")
+            log.error("Exception raised when calling eventix")
             log.exception(e)
             log.error("Exception used this task info")
             log.error(task.json())
 
         return None
```

### Comparing `eventix-0.2.0/eventix/pydantic/task.py` & `eventix-0.3.0/eventix/pydantic/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.2.0/eventix/router/event.py` & `eventix-0.3.0/eventix/router/event.py`

 * *Files identical despite different names*

### Comparing `eventix-0.2.0/eventix/router/task.py` & `eventix-0.3.0/eventix/router/task.py`

 * *Files identical despite different names*

### Comparing `eventix-0.2.0/pyproject.toml` & `eventix-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventix"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.95.1"
```

### Comparing `eventix-0.2.0/PKG-INFO` & `eventix-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventix
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
```

