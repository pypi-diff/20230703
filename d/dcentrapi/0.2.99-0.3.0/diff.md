# Comparing `tmp/dcentrapi-0.2.99.tar.gz` & `tmp/dcentrapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.99.tar", last modified: Wed Jun 28 07:00:34 2023, max compression
+gzip compressed data, was "dcentrapi-0.3.0.tar", last modified: Mon Jul  3 11:38:24 2023, max compression
```

## Comparing `dcentrapi-0.2.99.tar` & `dcentrapi-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-28 07:00:34.677385 dcentrapi-0.2.99/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.99/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-28 07:00:34.677235 dcentrapi-0.2.99/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.99/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-28 07:00:34.675855 dcentrapi-0.2.99/dcentrapi/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      771 2023-06-28 06:59:23.000000 dcentrapi-0.2.99/dcentrapi/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      397 2023-06-27 14:44:06.000000 dcentrapi-0.2.99/dcentrapi/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      130 2023-06-27 13:48:08.000000 dcentrapi-0.2.99/dcentrapi/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     8761 2023-06-27 14:44:57.000000 dcentrapi-0.2.99/dcentrapi/eventPolling.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      525 2023-06-27 14:44:57.000000 dcentrapi-0.2.99/dcentrapi/gasMonitor.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      561 2023-06-28 06:33:24.000000 dcentrapi-0.2.99/dcentrapi/hackMitigation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.99/dcentrapi/merkleTree.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      246 2023-06-28 07:00:24.000000 dcentrapi-0.2.99/dcentrapi/requests_dappi.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3107 2023-06-27 14:44:58.000000 dcentrapi-0.2.99/dcentrapi/rpcAggregation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      837 2023-06-27 14:44:59.000000 dcentrapi-0.2.99/dcentrapi/web3Index.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-28 07:00:34.677016 dcentrapi-0.2.99/dcentrapi.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6781 2023-06-28 07:00:34.000000 dcentrapi-0.2.99/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      435 2023-06-28 07:00:34.000000 dcentrapi-0.2.99/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-28 07:00:34.000000 dcentrapi-0.2.99/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-28 07:00:34.000000 dcentrapi-0.2.99/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-06-28 07:00:34.000000 dcentrapi-0.2.99/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-06-28 07:00:34.677523 dcentrapi-0.2.99/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1110 2023-06-28 06:59:17.000000 dcentrapi-0.2.99/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-07-03 11:38:24.548344 dcentrapi-0.3.0/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.3.0/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-07-03 11:38:24.548210 dcentrapi-0.3.0/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.3.0/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-07-03 11:38:24.547293 dcentrapi-0.3.0/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      903 2023-07-03 08:28:48.000000 dcentrapi-0.3.0/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      434 2023-07-03 08:17:20.000000 dcentrapi-0.3.0/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)     8761 2023-06-28 06:59:47.000000 dcentrapi-0.3.0/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      673 2023-07-03 08:17:20.000000 dcentrapi-0.3.0/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)      561 2023-07-03 08:19:01.000000 dcentrapi-0.3.0/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.3.0/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)      226 2023-06-28 06:59:47.000000 dcentrapi-0.3.0/dcentrapi/requests_dappi.py
+-rw-r--r--   0 oded       (502) staff       (20)     3107 2023-06-28 06:59:47.000000 dcentrapi-0.3.0/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.3.0/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)      837 2023-06-28 06:59:47.000000 dcentrapi-0.3.0/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-07-03 11:38:24.548010 dcentrapi-0.3.0/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      433 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-07-03 11:38:24.000000 dcentrapi-0.3.0/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-07-03 11:38:24.548384 dcentrapi-0.3.0/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1109 2023-07-03 08:22:17.000000 dcentrapi-0.3.0/setup.py
```

### Comparing `dcentrapi-0.2.99/LICENSE.rst` & `dcentrapi-0.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.99/PKG-INFO` & `dcentrapi-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.99
+Version: 0.3.0
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.99/README.md` & `dcentrapi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.99/dcentrapi/Base.py` & `dcentrapi-0.3.0/dcentrapi/Base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 class Base:
     def __init__(self, stage, username=None, key=None):
-        self.__version__ = "0.2.99"
+        self.__version__ = "0.3.0"
 
         if stage == "develop":
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://test-api.dcentralab.com/"
             self.web3index_url = "https://test-api.web3index.info/"
         if stage == "staging":
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://staging.dcentralab.com/"
             self.web3index_url = "https://staging-api.web3index.info/"
         if stage == "main":
             self.headers = {"Authorization": username + "," + key}
             self.url = "https://main-api.dcentralab.com/"
             self.web3index_url = "https://api.web3index.info/"
+
+
+class DapiError:
+    def __init__(self, response, exception):
+        self.response = response
+        self.exception = exception
+
```

### Comparing `dcentrapi-0.2.99/dcentrapi/eventPolling.py` & `dcentrapi-0.3.0/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.99/dcentrapi/gasMonitor.py` & `dcentrapi-0.3.0/dcentrapi/gasMonitor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from dcentrapi.Base import Base
+from dcentrapi.Base import Base, DapiError
 from dcentrapi.requests_dappi import requests_get
 
 
 class GasMonitor(Base):
 
     def get_optimal_gas_price(self, network_name, minutes, stats=None, values=None):
         url = self.url + "gas_monitor/optimal_gas_price_for_network"
         data = {
             "network_name": network_name,
             "minutes": minutes,
             "stats": stats,
             "values": values,
         }
-        response = requests_get(url, params=data, headers=self.headers)
-        return response.json()
+        response = None
+        try:
+            response = requests_get(url, params=data, headers=self.headers)
+            return response.json()
+        except Exception as e:
+            return DapiError(response=response, exception=e)
```

### Comparing `dcentrapi-0.2.99/dcentrapi/hackMitigation.py` & `dcentrapi-0.3.0/dcentrapi/hackMitigation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from dcentrapi.Base import Base
-from dcentrapi.common import DapiError
+from dcentrapi.Base import Base, DapiError
 from dcentrapi.requests_dappi import requests_get
 
 
 class HackMitigation(Base):
 
     def are_addresses_blacklisted(self, addresses: [str]):
         url = self.url + "generic_freeze_signal/are_addresses_blacklisted"
         data = {
             "addresses": addresses,
         }
-        response = requests_get(url, params=data, headers=self.headers)
+        response = None
         try:
+            response = requests_get(url, params=data, headers=self.headers)
             return response.json()
         except Exception as e:
             return DapiError(response=response, exception=e)
```

### Comparing `dcentrapi-0.2.99/dcentrapi/merkleTree.py` & `dcentrapi-0.3.0/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.99/dcentrapi/rpcAggregation.py` & `dcentrapi-0.3.0/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.99/dcentrapi/web3Index.py` & `dcentrapi-0.3.0/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.99/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.3.0/dcentrapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.99
+Version: 0.3.0
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.99/setup.py` & `dcentrapi-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return result.group(1)
 
 
 DESCRIPTION = 'Dcentralab Pypi packages'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 project_name = 'dcentrapi'
-VERSION = "0.2.99"
+VERSION = "0.3.0"
 
 
 # Setting up
 setup(
     name="dcentrapi",
     version=VERSION,
     author="Dcentralab (Niv Shitrit)",
```

