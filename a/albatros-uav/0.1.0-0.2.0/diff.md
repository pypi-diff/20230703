# Comparing `tmp/albatros_uav-0.1.0.tar.gz` & `tmp/albatros_uav-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albatros_uav-0.1.0.tar", max compression
+gzip compressed data, was "albatros_uav-0.2.0.tar", max compression
```

## Comparing `albatros_uav-0.1.0.tar` & `albatros_uav-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      251 2023-06-23 07:35:50.637081 albatros_uav-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-09 15:52:27.239088 albatros_uav-0.1.0/albatros/__init__.py
--rw-r--r--   0        0        0     5944 2023-06-11 08:27:47.442808 albatros_uav-0.1.0/albatros/commands.py
--rw-r--r--   0        0        0     7312 2023-06-11 08:27:47.443808 albatros_uav-0.1.0/albatros/enums.py
--rw-r--r--   0        0        0        0 2023-06-14 12:38:56.434756 albatros_uav-0.1.0/albatros/nav/__init__.py
--rw-r--r--   0        0        0     1410 2023-06-14 15:16:21.197023 albatros_uav-0.1.0/albatros/nav/position.py
--rw-r--r--   0        0        0     1852 2023-06-28 16:14:16.302180 albatros_uav-0.1.0/albatros/telemetry_source.py
--rw-r--r--   0        0        0     6455 2023-06-28 16:14:16.299180 albatros_uav-0.1.0/albatros/uav.py
--rw-r--r--   0        0        0      757 2023-06-28 16:22:01.922822 albatros_uav-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 albatros_uav-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2023-06-28 21:11:22.663227 albatros_uav-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 15:52:27.239088 albatros_uav-0.2.0/albatros/__init__.py
+-rw-r--r--   0        0        0     5944 2023-06-11 08:27:47.442808 albatros_uav-0.2.0/albatros/commands.py
+-rw-r--r--   0        0        0     7312 2023-06-11 08:27:47.443808 albatros_uav-0.2.0/albatros/enums.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:38:56.434756 albatros_uav-0.2.0/albatros/nav/__init__.py
+-rw-r--r--   0        0        0     1410 2023-06-14 15:16:21.197023 albatros_uav-0.2.0/albatros/nav/position.py
+-rw-r--r--   0        0        0     1814 2023-07-03 21:45:33.471753 albatros_uav-0.2.0/albatros/telemetry_source.py
+-rw-r--r--   0        0        0     6455 2023-07-03 21:45:33.472753 albatros_uav-0.2.0/albatros/uav.py
+-rw-r--r--   0        0        0      757 2023-07-03 21:50:32.664560 albatros_uav-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 albatros_uav-0.2.0/PKG-INFO
```

### Comparing `albatros_uav-0.1.0/albatros/commands.py` & `albatros_uav-0.2.0/albatros/commands.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.1.0/albatros/enums.py` & `albatros_uav-0.2.0/albatros/enums.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.1.0/albatros/nav/position.py` & `albatros_uav-0.2.0/albatros/nav/position.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.1.0/albatros/telemetry_source.py` & `albatros_uav-0.2.0/albatros/telemetry_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,15 @@
         if self.connection_type == ConnectionType.DIRECT:
             self.make_direct_connection()
 
         if self.connection_type == ConnectionType.RABBITMQ:
             self.make_rabbitmq_connection()
 
     def make_direct_connection(self) -> None:
-        self.direct_connection: mavutil.mavudp = mavutil.mavlink_connection(
-            self.device, self.baud_rate
-        )
+        self.direct_connection = mavutil.mavlink_connection(self.device, self.baud_rate)
         self.direct_connection.wait_heartbeat()
         logger.info("heartbeat recived")
 
     def make_rabbitmq_connection(self) -> None:
         connection = pika.BlockingConnection(pika.ConnectionParameters(self.host))
         self.rabbit_connection = connection.channel()
         self.rabbit_connection.queue_declare(queue="commands")
```

### Comparing `albatros_uav-0.1.0/albatros/uav.py` & `albatros_uav-0.2.0/albatros/uav.py`

 * *Files identical despite different names*

### Comparing `albatros_uav-0.1.0/pyproject.toml` & `albatros_uav-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "albatros-uav"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Jędrzej Stasik <sjedrzej58@gmail.com>"]
 readme = "README.md"
 packages = [{include = "albatros"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `albatros_uav-0.1.0/PKG-INFO` & `albatros_uav-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albatros-uav
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Jędrzej Stasik
 Author-email: sjedrzej58@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

