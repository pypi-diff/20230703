# Comparing `tmp/tailscale_localapi-0.1.0.tar.gz` & `tmp/tailscale_localapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailscale_localapi-0.1.0.tar", max compression
+gzip compressed data, was "tailscale_localapi-0.2.0.tar", max compression
```

## Comparing `tailscale_localapi-0.1.0.tar` & `tailscale_localapi-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-03 09:10:32.160699 tailscale_localapi-0.1.0/LICENSE
--rw-r--r--   0        0        0      350 2023-07-03 09:13:57.307226 tailscale_localapi-0.1.0/README.md
--rw-r--r--   0        0        0      519 2023-07-03 09:14:42.713866 tailscale_localapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-07-03 09:11:19.040664 tailscale_localapi-0.1.0/tailscale_localapi/__init__.py
--rw-r--r--   0        0        0       46 2023-07-03 09:11:19.040664 tailscale_localapi-0.1.0/tailscale_localapi/_util/error.py
--rw-r--r--   0        0        0      771 2023-07-03 09:11:19.040664 tailscale_localapi-0.1.0/tailscale_localapi/_util/sock.py
--rw-r--r--   0        0        0      654 2023-07-03 09:11:19.040664 tailscale_localapi-0.1.0/tailscale_localapi/api.py
--rw-r--r--   0        0        0       34 2023-07-03 09:11:19.040664 tailscale_localapi-0.1.0/tailscale_localapi/v0/__init__.py
--rw-r--r--   0        0        0     3713 2023-07-03 09:11:19.040664 tailscale_localapi-0.1.0/tailscale_localapi/v0/api.py
--rw-r--r--   0        0        0     1872 2023-07-03 09:11:19.040664 tailscale_localapi-0.1.0/tailscale_localapi/v0/config.py
--rw-r--r--   0        0        0     2103 2023-07-03 09:11:19.040664 tailscale_localapi-0.1.0/tailscale_localapi/v0/peers.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 tailscale_localapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-03 09:10:32.160699 tailscale_localapi-0.2.0/LICENSE
+-rw-r--r--   0        0        0      350 2023-07-03 09:13:57.307226 tailscale_localapi-0.2.0/README.md
+-rw-r--r--   0        0        0      519 2023-07-03 09:40:43.710236 tailscale_localapi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-07-03 09:40:38.150249 tailscale_localapi-0.2.0/tailscale_localapi/__init__.py
+-rw-r--r--   0        0        0       46 2023-07-03 09:11:19.040664 tailscale_localapi-0.2.0/tailscale_localapi/_util/error.py
+-rw-r--r--   0        0        0      771 2023-07-03 09:11:19.040664 tailscale_localapi-0.2.0/tailscale_localapi/_util/sock.py
+-rw-r--r--   0        0        0      654 2023-07-03 09:11:19.040664 tailscale_localapi-0.2.0/tailscale_localapi/api.py
+-rw-r--r--   0        0        0       34 2023-07-03 09:11:19.040664 tailscale_localapi-0.2.0/tailscale_localapi/v0/__init__.py
+-rw-r--r--   0        0        0     3713 2023-07-03 09:11:19.040664 tailscale_localapi-0.2.0/tailscale_localapi/v0/api.py
+-rw-r--r--   0        0        0     1872 2023-07-03 09:11:19.040664 tailscale_localapi-0.2.0/tailscale_localapi/v0/config.py
+-rw-r--r--   0        0        0     2103 2023-07-03 09:11:19.040664 tailscale_localapi-0.2.0/tailscale_localapi/v0/peers.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 tailscale_localapi-0.2.0/PKG-INFO
```

### Comparing `tailscale_localapi-0.1.0/LICENSE` & `tailscale_localapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tailscale_localapi-0.1.0/pyproject.toml` & `tailscale_localapi-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tailscale_localapi"
-version = "0.1.0"
+version = "0.2.0"
 description = "Control Tailscale's local socket API"
 authors = ["Antoine POPINEAU <antoine@popineau.eu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tailscale_localapi"}]
 
 [tool.poetry.dependencies]
```

### Comparing `tailscale_localapi-0.1.0/tailscale_localapi/_util/sock.py` & `tailscale_localapi-0.2.0/tailscale_localapi/_util/sock.py`

 * *Files identical despite different names*

### Comparing `tailscale_localapi-0.1.0/tailscale_localapi/api.py` & `tailscale_localapi-0.2.0/tailscale_localapi/api.py`

 * *Files identical despite different names*

### Comparing `tailscale_localapi-0.1.0/tailscale_localapi/v0/api.py` & `tailscale_localapi-0.2.0/tailscale_localapi/v0/api.py`

 * *Files identical despite different names*

### Comparing `tailscale_localapi-0.1.0/tailscale_localapi/v0/config.py` & `tailscale_localapi-0.2.0/tailscale_localapi/v0/config.py`

 * *Files identical despite different names*

### Comparing `tailscale_localapi-0.1.0/tailscale_localapi/v0/peers.py` & `tailscale_localapi-0.2.0/tailscale_localapi/v0/peers.py`

 * *Files identical despite different names*

### Comparing `tailscale_localapi-0.1.0/PKG-INFO` & `tailscale_localapi-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailscale-localapi
-Version: 0.1.0
+Version: 0.2.0
 Summary: Control Tailscale's local socket API
 License: MIT
 Author: Antoine POPINEAU
 Author-email: antoine@popineau.eu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

