# Comparing `tmp/model2queue-0.1.5.tar.gz` & `tmp/model2queue-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model2queue-0.1.5.tar", last modified: Thu May 11 14:54:37 2023, max compression
+gzip compressed data, was "model2queue-0.1.6.tar", last modified: Mon Jul  3 13:19:50 2023, max compression
```

## Comparing `model2queue-0.1.5.tar` & `model2queue-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:54:37.679848 model2queue-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-11 14:54:37.679848 model2queue-0.1.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:54:37.679848 model2queue-0.1.5/model2queue/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/api_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:54:37.679848 model2queue-0.1.5/model2queue/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:54:37.679848 model2queue-0.1.5/model2queue/examples/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/examples/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/examples/fastapi/preprocess_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/examples/fastapi/simple_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:54:37.679848 model2queue-0.1.5/model2queue/helper/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/helper/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:54:37.679848 model2queue-0.1.5/model2queue/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/workers/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/workers/consumer_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-11 14:54:27.000000 model2queue-0.1.5/model2queue/workers/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:54:37.679848 model2queue-0.1.5/model2queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-11 14:54:37.000000 model2queue-0.1.5/model2queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-11 14:54:37.000000 model2queue-0.1.5/model2queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:54:37.000000 model2queue-0.1.5/model2queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 14:54:37.000000 model2queue-0.1.5/model2queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 14:54:37.000000 model2queue-0.1.5/model2queue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:54:37.679848 model2queue-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-11 14:54:27.000000 model2queue-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:19:50.788786 model2queue-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-03 13:19:50.788786 model2queue-0.1.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:19:50.784786 model2queue-0.1.6/model2queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/api_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:19:50.784786 model2queue-0.1.6/model2queue/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:19:50.788786 model2queue-0.1.6/model2queue/examples/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/examples/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/examples/fastapi/preprocess_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/examples/fastapi/simple_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:19:50.788786 model2queue-0.1.6/model2queue/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/helper/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:19:50.788786 model2queue-0.1.6/model2queue/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/workers/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/workers/consumer_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 13:19:42.000000 model2queue-0.1.6/model2queue/workers/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:19:50.784786 model2queue-0.1.6/model2queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-03 13:19:50.000000 model2queue-0.1.6/model2queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-03 13:19:50.000000 model2queue-0.1.6/model2queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:19:50.000000 model2queue-0.1.6/model2queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-03 13:19:50.000000 model2queue-0.1.6/model2queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 13:19:50.000000 model2queue-0.1.6/model2queue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:19:50.788786 model2queue-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 13:19:42.000000 model2queue-0.1.6/setup.py
```

### Comparing `model2queue-0.1.5/model2queue/api_tasks.py` & `model2queue-0.1.6/model2queue/api_tasks.py`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.5/model2queue/examples/fastapi/preprocess_images.py` & `model2queue-0.1.6/model2queue/examples/fastapi/preprocess_images.py`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.5/model2queue/examples/fastapi/simple_model.py` & `model2queue-0.1.6/model2queue/examples/fastapi/simple_model.py`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.5/model2queue/workers/consumer.py` & `model2queue-0.1.6/model2queue/workers/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.n_workers = n_workers
 
     def get_consumers(self, consumer: Consumer, channel: Any) -> List[Consumer]:
         return [
             consumer(
                 queues=self.queue,
                 on_message=self.handle_message,
-                prefetch_count=10,
+                prefetch_count=1,
             )
             for _ in range(self.n_workers)
         ]
 
     def handle_message(self, message: Message) -> None:
         logger.debug(f"received {message} from {self.queue}")
         try:
```

### Comparing `model2queue-0.1.5/model2queue/workers/consumer_producer.py` & `model2queue-0.1.6/model2queue/workers/consumer_producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.n_workers = n_workers
 
     def get_consumers(self, consumer: Consumer, channel: Any) -> List[Consumer]:
         return [
             consumer(
                 queues=self.queue,
                 on_message=self.handle_message,
-                prefetch_count=10,
+                prefetch_count=1,
             )
             for _ in range(self.n_workers)
         ]
 
     def handle_message(self, message: Message) -> None:
         logger.debug(f"received {message} from {self.queue}")
         output = self.callback_function(message.payload)
```

### Comparing `model2queue-0.1.5/model2queue.egg-info/SOURCES.txt` & `model2queue-0.1.6/model2queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `model2queue-0.1.5/setup.py` & `model2queue-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="model2queue",
     packages=find_packages(),
-    version="0.1.5",
+    version="0.1.6",
     description="A library to expose an api with a queue for batch predictions",
     author="collective.ai",
     author_email="team.collective.ai@gmail.com",
     url="https://github.com/collectiveai-team/model2queue",
     install_requires=["kombu", "fastapi", "uvicorn", "rich"],
     package_data={"": ["*.yml", "*.yaml"]},
     include_package_data=True,
```

