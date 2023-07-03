# Comparing `tmp/web3mc-0.1.3.tar.gz` & `tmp/web3mc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3mc-0.1.3.tar", max compression
+gzip compressed data, was "web3mc-0.1.4.tar", max compression
```

## Comparing `web3mc-0.1.3.tar` & `web3mc-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1056 2023-07-03 00:49:32.332797 web3mc-0.1.3/LICENSE
--rw-r--r--   0        0        0     2649 2023-07-03 00:49:32.332797 web3mc-0.1.3/README.md
--rw-r--r--   0        0        0      807 2023-07-03 00:49:32.332797 web3mc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       58 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/__init__.py
--rw-r--r--   0        0        0    14532 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/abi.py
--rw-r--r--   0        0        0       58 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/auto.py
--rw-r--r--   0        0        0     1545 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/call.py
--rw-r--r--   0        0        0    20758 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/constants.py
--rw-r--r--   0        0        0       46 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/exceptions.py
--rw-r--r--   0        0        0     7739 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/multicall.py
--rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 web3mc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-07-03 01:07:20.140872 web3mc-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2649 2023-07-03 01:07:20.140872 web3mc-0.1.4/README.md
+-rw-r--r--   0        0        0      807 2023-07-03 01:07:20.140872 web3mc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/__init__.py
+-rw-r--r--   0        0        0    14532 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/abi.py
+-rw-r--r--   0        0        0       58 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/auto.py
+-rw-r--r--   0        0        0     1545 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/call.py
+-rw-r--r--   0        0        0    20758 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/constants.py
+-rw-r--r--   0        0        0       46 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/exceptions.py
+-rw-r--r--   0        0        0     7739 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/multicall.py
+-rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 web3mc-0.1.4/PKG-INFO
```

### Comparing `web3mc-0.1.3/LICENSE` & `web3mc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.3/README.md` & `web3mc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.3/pyproject.toml` & `web3mc-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web3mc"
-version = "0.1.3"
+version = "0.1.4"
 description = "Multicall library for aggregating web3py contract calls"
 authors = ["amfet42"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `web3mc-0.1.3/web3mc/abi.py` & `web3mc-0.1.4/web3mc/abi.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.3/web3mc/call.py` & `web3mc-0.1.4/web3mc/call.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.3/web3mc/constants.py` & `web3mc-0.1.4/web3mc/constants.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.3/web3mc/multicall.py` & `web3mc-0.1.4/web3mc/multicall.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.3/PKG-INFO` & `web3mc-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3mc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Multicall library for aggregating web3py contract calls
 License: MIT
 Author: amfet42
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

