# Comparing `tmp/web3mc-0.1.0.tar.gz` & `tmp/web3mc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3mc-0.1.0.tar", max compression
+gzip compressed data, was "web3mc-0.1.3.tar", max compression
```

## Comparing `web3mc-0.1.0.tar` & `web3mc-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1056 2023-07-02 21:52:17.569372 web3mc-0.1.0/LICENSE
--rw-r--r--   0        0        0     2684 2023-07-02 21:58:13.835710 web3mc-0.1.0/README.md
--rw-r--r--   0        0        0      807 2023-07-02 21:56:00.156192 web3mc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       58 2023-07-02 21:52:17.572194 web3mc-0.1.0/web3mc/__init__.py
--rw-r--r--   0        0        0    14532 2023-07-02 21:52:17.572534 web3mc-0.1.0/web3mc/abi.py
--rw-r--r--   0        0        0       58 2023-07-02 21:52:17.572765 web3mc-0.1.0/web3mc/auto.py
--rw-r--r--   0        0        0     1545 2023-07-02 21:52:17.572992 web3mc-0.1.0/web3mc/call.py
--rw-r--r--   0        0        0    20758 2023-07-02 21:52:17.573423 web3mc-0.1.0/web3mc/constants.py
--rw-r--r--   0        0        0       46 2023-07-02 21:52:17.573659 web3mc-0.1.0/web3mc/exceptions.py
--rw-r--r--   0        0        0     7739 2023-07-02 21:52:17.573870 web3mc-0.1.0/web3mc/multicall.py
--rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 web3mc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-07-03 00:49:32.332797 web3mc-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2649 2023-07-03 00:49:32.332797 web3mc-0.1.3/README.md
+-rw-r--r--   0        0        0      807 2023-07-03 00:49:32.332797 web3mc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/__init__.py
+-rw-r--r--   0        0        0    14532 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/abi.py
+-rw-r--r--   0        0        0       58 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/auto.py
+-rw-r--r--   0        0        0     1545 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/call.py
+-rw-r--r--   0        0        0    20758 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/constants.py
+-rw-r--r--   0        0        0       46 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/exceptions.py
+-rw-r--r--   0        0        0     7739 2023-07-03 00:49:32.332797 web3mc-0.1.3/web3mc/multicall.py
+-rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 web3mc-0.1.3/PKG-INFO
```

### Comparing `web3mc-0.1.0/LICENSE` & `web3mc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.0/README.md` & `web3mc-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Based on makerdao's [multicall contract](https://github.com/makerdao/multicall)and
 [brownie](https://github.com/eth-brownie/brownie) implementation with batching and asynchronous support. Works
 directly with web3py contract functions and parameters
 
 ## Installation
 
 ```shell
-pip install git+https://github.com/amfet42/web3mc.git
+pip install web3mc
 ```
 
 ## Quickstart
 
 Basic usage
 
 (this is default value if empty - set by web3py)
```

### Comparing `web3mc-0.1.0/pyproject.toml` & `web3mc-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web3mc"
-version = "0.1.0"
+version = "0.1.3"
 description = "Multicall library for aggregating web3py contract calls"
 authors = ["amfet42"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `web3mc-0.1.0/web3mc/abi.py` & `web3mc-0.1.3/web3mc/abi.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.0/web3mc/call.py` & `web3mc-0.1.3/web3mc/call.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.0/web3mc/constants.py` & `web3mc-0.1.3/web3mc/constants.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.0/web3mc/multicall.py` & `web3mc-0.1.3/web3mc/multicall.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.0/PKG-INFO` & `web3mc-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3mc
-Version: 0.1.0
+Version: 0.1.3
 Summary: Multicall library for aggregating web3py contract calls
 License: MIT
 Author: amfet42
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -17,15 +17,15 @@
 Based on makerdao's [multicall contract](https://github.com/makerdao/multicall)and
 [brownie](https://github.com/eth-brownie/brownie) implementation with batching and asynchronous support. Works
 directly with web3py contract functions and parameters
 
 ## Installation
 
 ```shell
-pip install git+https://github.com/amfet42/web3mc.git
+pip install web3mc
 ```
 
 ## Quickstart
 
 Basic usage
 
 (this is default value if empty - set by web3py)
```

