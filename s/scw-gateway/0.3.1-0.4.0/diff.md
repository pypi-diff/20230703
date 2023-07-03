# Comparing `tmp/scw_gateway-0.3.1.tar.gz` & `tmp/scw_gateway-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scw_gateway-0.3.1.tar", max compression
+gzip compressed data, was "scw_gateway-0.4.0.tar", max compression
```

## Comparing `scw_gateway-0.3.1.tar` & `scw_gateway-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
--rw-r--r--   0        0        0        0 2023-06-27 07:57:20.419057 scw_gateway-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-27 07:57:20.419057 scw_gateway-0.3.1/cli/__init__.py
--rw-r--r--   0        0        0     4952 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/cli.py
--rw-r--r--   0        0        0      352 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/client.py
--rw-r--r--   0        0        0     2465 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/conf.py
--rw-r--r--   0        0        0     5707 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/gateway.py
--rw-r--r--   0        0        0      281 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/__init__.py
--rw-r--r--   0        0        0     1978 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/cockpit.py
--rw-r--r--   0        0        0     6009 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/container.py
--rw-r--r--   0        0        0      519 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/function.py
--rw-r--r--   0        0        0      317 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/image.py
--rw-r--r--   0        0        0    15463 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/manager.py
--rw-r--r--   0        0        0      999 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/rdb.py
--rw-r--r--   0        0        0     2515 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/infra/secrets.py
--rw-r--r--   0        0        0     1037 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/cli/model.py
--rw-r--r--   0        0        0      923 2023-06-27 07:57:20.423057 scw_gateway-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 scw_gateway-0.3.1/setup.py
--rw-r--r--   0        0        0      622 1970-01-01 00:00:00.000000 scw_gateway-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2979 2023-07-03 14:54:01.781895 scw_gateway-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/__init__.py
+-rw-r--r--   0        0        0      825 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/cli.py
+-rw-r--r--   0        0        0      352 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/client.py
+-rw-r--r--   0        0        0      616 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/consumer.py
+-rw-r--r--   0        0        0      758 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/dev.py
+-rw-r--r--   0        0        0     2958 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/infra.py
+-rw-r--r--   0        0        0      538 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/jwt.py
+-rw-r--r--   0        0        0     1575 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/commands/route.py
+-rw-r--r--   0        0        0     2465 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/conf.py
+-rw-r--r--   0        0        0     8041 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/gateway.py
+-rw-r--r--   0        0        0      281 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/__init__.py
+-rw-r--r--   0        0        0     1978 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/cockpit.py
+-rw-r--r--   0        0        0     6009 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/container.py
+-rw-r--r--   0        0        0      519 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/function.py
+-rw-r--r--   0        0        0      317 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/image.py
+-rw-r--r--   0        0        0    15463 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/manager.py
+-rw-r--r--   0        0        0      999 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/rdb.py
+-rw-r--r--   0        0        0     2515 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/infra/secrets.py
+-rw-r--r--   0        0        0     1901 2023-07-03 14:53:22.501477 scw_gateway-0.4.0/cli/model.py
+-rw-r--r--   0        0        0      940 2023-07-03 14:53:22.505477 scw_gateway-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 scw_gateway-0.4.0/setup.py
+-rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 scw_gateway-0.4.0/PKG-INFO
```

### Comparing `scw_gateway-0.3.1/cli/conf.py` & `scw_gateway-0.4.0/cli/conf.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.1/cli/infra/cockpit.py` & `scw_gateway-0.4.0/cli/infra/cockpit.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.1/cli/infra/container.py` & `scw_gateway-0.4.0/cli/infra/container.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.1/cli/infra/function.py` & `scw_gateway-0.4.0/cli/infra/function.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.1/cli/infra/manager.py` & `scw_gateway-0.4.0/cli/infra/manager.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.1/cli/infra/rdb.py` & `scw_gateway-0.4.0/cli/infra/rdb.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.1/cli/infra/secrets.py` & `scw_gateway-0.4.0/cli/infra/secrets.py`

 * *Files identical despite different names*

### Comparing `scw_gateway-0.3.1/pyproject.toml` & `scw_gateway-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scw-gateway"
-version = "0.3.1"
+version = "0.4.0"
 description = "CLI to deploy and manage a self-hosted Kong gateway on Scaleway Serverless Ecosystem"
 authors = ["Simon Shillaker <sshillaker@scaleway.com>"]
 readme = "README.md"
 packages = [{ include = "cli" }]
 
 [tool.poetry.dependencies]
 loguru = "0.6.0"
@@ -14,15 +14,16 @@
 pyyaml = "^6.0"
 scaleway = "^0.12.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
-mypy = "^1.2.0"
+mypy = "^1.4.1"
+pyjwt = "^2.7.0"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 responses = "^0.23.1"
 types-pyyaml = "^6.0.12.9"
 types-requests = "^2.29.0.0"
 
 [build-system]
```

