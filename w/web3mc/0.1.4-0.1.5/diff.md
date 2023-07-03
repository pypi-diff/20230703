# Comparing `tmp/web3mc-0.1.4.tar.gz` & `tmp/web3mc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3mc-0.1.4.tar", max compression
+gzip compressed data, was "web3mc-0.1.5.tar", max compression
```

## Comparing `web3mc-0.1.4.tar` & `web3mc-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1056 2023-07-03 01:07:20.140872 web3mc-0.1.4/LICENSE
--rw-r--r--   0        0        0     2649 2023-07-03 01:07:20.140872 web3mc-0.1.4/README.md
--rw-r--r--   0        0        0      807 2023-07-03 01:07:20.140872 web3mc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       58 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/__init__.py
--rw-r--r--   0        0        0    14532 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/abi.py
--rw-r--r--   0        0        0       58 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/auto.py
--rw-r--r--   0        0        0     1545 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/call.py
--rw-r--r--   0        0        0    20758 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/constants.py
--rw-r--r--   0        0        0       46 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/exceptions.py
--rw-r--r--   0        0        0     7739 2023-07-03 01:07:20.140872 web3mc-0.1.4/web3mc/multicall.py
--rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 web3mc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-07-03 01:13:51.284056 web3mc-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2649 2023-07-03 01:13:51.284056 web3mc-0.1.5/README.md
+-rw-r--r--   0        0        0      889 2023-07-03 01:13:51.288056 web3mc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-07-03 01:13:51.288056 web3mc-0.1.5/web3mc/__init__.py
+-rw-r--r--   0        0        0    14532 2023-07-03 01:13:51.288056 web3mc-0.1.5/web3mc/abi.py
+-rw-r--r--   0        0        0       58 2023-07-03 01:13:51.288056 web3mc-0.1.5/web3mc/auto.py
+-rw-r--r--   0        0        0     1545 2023-07-03 01:13:51.288056 web3mc-0.1.5/web3mc/call.py
+-rw-r--r--   0        0        0    20758 2023-07-03 01:13:51.288056 web3mc-0.1.5/web3mc/constants.py
+-rw-r--r--   0        0        0       46 2023-07-03 01:13:51.288056 web3mc-0.1.5/web3mc/exceptions.py
+-rw-r--r--   0        0        0     7739 2023-07-03 01:13:51.288056 web3mc-0.1.5/web3mc/multicall.py
+-rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 web3mc-0.1.5/PKG-INFO
```

### Comparing `web3mc-0.1.4/LICENSE` & `web3mc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.4/README.md` & `web3mc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.4/web3mc/abi.py` & `web3mc-0.1.5/web3mc/abi.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.4/web3mc/call.py` & `web3mc-0.1.5/web3mc/call.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.4/web3mc/constants.py` & `web3mc-0.1.5/web3mc/constants.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.4/web3mc/multicall.py` & `web3mc-0.1.5/web3mc/multicall.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.4/PKG-INFO` & `web3mc-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: web3mc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Multicall library for aggregating web3py contract calls
+Home-page: https://github.com/amfet42/web3mc
 License: MIT
+Keywords: web3,multicall
 Author: amfet42
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: web3 (>=6.0.0)
+Project-URL: Repository, https://github.com/amfet42/web3mc
 Description-Content-Type: text/markdown
 
 # web3mc - multicall library for web3py
 
 Based on makerdao's [multicall contract](https://github.com/makerdao/multicall)and
 [brownie](https://github.com/eth-brownie/brownie) implementation with batching and asynchronous support. Works
 directly with web3py contract functions and parameters
```

