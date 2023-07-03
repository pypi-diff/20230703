# Comparing `tmp/pwebserver-23.6a0.tar.gz` & `tmp/pwebserver-23.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwebserver-23.6a0.tar", last modified: Sun Jul  2 23:44:13 2023, max compression
+gzip compressed data, was "pwebserver-23.6a1.tar", last modified: Mon Jul  3 19:43:22 2023, max compression
```

## Comparing `pwebserver-23.6a0.tar` & `pwebserver-23.6a1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-07-01 14:48:08.320142 pwebserver-23.6a0/LICENSE
--rw-r--r--   0        0        0      693 2023-07-02 19:48:52.096813 pwebserver-23.6a0/README.md
--rw-r--r--   0        0        0      538 2023-07-02 23:44:13.276321 pwebserver-23.6a0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-02 17:29:35.519402 pwebserver-23.6a0/src/__init__.py
--rw-r--r--   0        0        0     5944 2023-07-02 20:07:36.262705 pwebserver-23.6a0/src/server.py
--rw-r--r--   0        0        0        0 2023-06-29 12:26:40.578357 pwebserver-23.6a0/tests/__init__.py
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 pwebserver-23.6a0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-01 14:48:08.320142 pwebserver-23.6a1/LICENSE
+-rw-r--r--   0        0        0     1931 2023-07-03 19:41:28.463538 pwebserver-23.6a1/README.md
+-rw-r--r--   0        0        0      584 2023-07-03 19:43:22.408376 pwebserver-23.6a1/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-03 17:08:59.174050 pwebserver-23.6a1/src/__init__.py
+-rw-r--r--   0        0        0     8743 2023-07-03 19:35:45.362734 pwebserver-23.6a1/src/pWebServer.py
+-rw-r--r--   0        0        0        0 2023-06-29 12:26:40.578357 pwebserver-23.6a1/tests/__init__.py
+-rw-r--r--   0        0        0      883 2023-07-03 18:55:17.870312 pwebserver-23.6a1/tests/test_server.py
+-rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 pwebserver-23.6a1/PKG-INFO
```

### Comparing `pwebserver-23.6a0/LICENSE` & `pwebserver-23.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pwebserver-23.6a0/pyproject.toml` & `pwebserver-23.6a1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pWebServer"
-version = "23.6a"
+version = "23.6a1"
 description = "Small, asynchronous web server for use with Raspberry Pi Pico W boards and similar"
 authors = [
     { name = "Stephen Sadowski", email = "stephen.sadowski@sjsadowski.com" },
 ]
 dependencies = []
 requires-python = ">=3.11"
 readme = "README.md"
@@ -17,10 +17,15 @@
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.4.0",
-    "pytest-aio>=1.5.0",
-    "pytest-aiohttp-client>=0.1.0",
+    "pytest-asyncio>=0.21.0",
+    "httpx>=0.24.1",
+]
+
+[tool.pytest.ini_options]
+pythonpath = [
+    "src",
 ]
```

