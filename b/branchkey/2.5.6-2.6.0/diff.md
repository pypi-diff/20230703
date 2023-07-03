# Comparing `tmp/branchkey-2.5.6.tar.gz` & `tmp/branchkey-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "branchkey-2.5.6.tar", last modified: Tue May 30 11:02:28 2023, max compression
+gzip compressed data, was "branchkey-2.6.0.tar", last modified: Mon Jul  3 11:25:41 2023, max compression
```

## Comparing `branchkey-2.5.6.tar` & `branchkey-2.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:02:28.402993 branchkey-2.5.6/
--rw-r--r--   0 root         (0) root         (0)     5342 2023-05-30 11:02:28.402993 branchkey-2.5.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4810 2023-05-25 09:40:36.000000 branchkey-2.5.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-05-25 09:40:36.000000 branchkey-2.5.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 11:02:28.402993 branchkey-2.5.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-30 11:02:27.000000 branchkey-2.5.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:02:28.402993 branchkey-2.5.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:02:28.402993 branchkey-2.5.6/src/branchkey/
--rw-rw-rw-   0 root         (0) root         (0)     5125 2023-05-25 09:40:36.000000 branchkey-2.5.6/src/branchkey/__consumer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 09:40:36.000000 branchkey-2.5.6/src/branchkey/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10685 2023-05-30 11:02:16.000000 branchkey-2.5.6/src/branchkey/client.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-25 09:40:36.000000 branchkey-2.5.6/src/branchkey/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:02:28.402993 branchkey-2.5.6/src/branchkey.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5342 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 11:02:28.000000 branchkey-2.5.6/src/branchkey.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:25:41.704577 branchkey-2.6.0/
+-rw-r--r--   0 root         (0) root         (0)     5243 2023-07-03 11:25:41.704577 branchkey-2.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4711 2023-07-03 11:25:26.000000 branchkey-2.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-05-25 09:44:56.000000 branchkey-2.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 11:25:41.704577 branchkey-2.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-03 11:25:40.000000 branchkey-2.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:25:41.692577 branchkey-2.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:25:41.692577 branchkey-2.6.0/src/branchkey/
+-rw-rw-rw-   0 root         (0) root         (0)     5125 2023-05-25 09:44:56.000000 branchkey-2.6.0/src/branchkey/__consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 09:44:56.000000 branchkey-2.6.0/src/branchkey/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10466 2023-07-03 11:25:26.000000 branchkey-2.6.0/src/branchkey/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-25 09:44:56.000000 branchkey-2.6.0/src/branchkey/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:25:41.704577 branchkey-2.6.0/src/branchkey.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5243 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-03 11:25:41.000000 branchkey-2.6.0/src/branchkey.egg-info/top_level.txt
```

### Comparing `branchkey-2.5.6/PKG-INFO` & `branchkey-2.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branchkey
-Version: 2.5.6
+Version: 2.6.0
 Summary: Client application to interface with the BranchKey system
 Home-page: https://branchkey.com
 Author: BranchKey
 Author-email: info@branchkey.com
 Project-URL: Homepage, https://branchkey.com
 Project-URL: Repository, https://gitlab.com/branchkey/client_application
 Classifier: Programming Language :: Python :: 3
@@ -41,25 +41,24 @@
   ```python
   import json
   from branchkey.client import Client
 
   credentials = {"leaf_name": "leaf-1",
                  "leaf_id": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "leaf_session_token": "46780841-9787-41e6-ac14-e3ee160e158a",
-                 "performance_analyser_username": "hello",
-                 "performance_analyser_password": "world",
                  "response_host":"response.branchkey.com"}
 
   host = "http://api.branchkey.com"
 
   '''initialise the client
   it implicitly authenticates the leaf_session
   and fetches the run_details of the parent branch
 
-  ssl: Whether to verify the SSL certificates of the remote host or not
+  ssl: Whether to verify the SSL certificates of the
+  remote host or not. Default it True
 
   wait_for_run: When trying to upload file, if the
   run is stopped/paused, this parameter decides whether
   to throw exception and stop the process, or wait for
   the run to be started again. Default is False
 
   run_check_interval_s: if wait_for_run=True, this
```

### Comparing `branchkey-2.5.6/README.md` & `branchkey-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,24 @@
   ```python
   import json
   from branchkey.client import Client
 
   credentials = {"leaf_name": "leaf-1",
                  "leaf_id": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "leaf_session_token": "46780841-9787-41e6-ac14-e3ee160e158a",
-                 "performance_analyser_username": "hello",
-                 "performance_analyser_password": "world",
                  "response_host":"response.branchkey.com"}
 
   host = "http://api.branchkey.com"
 
   '''initialise the client
   it implicitly authenticates the leaf_session
   and fetches the run_details of the parent branch
 
-  ssl: Whether to verify the SSL certificates of the remote host or not
+  ssl: Whether to verify the SSL certificates of the
+  remote host or not. Default it True
 
   wait_for_run: When trying to upload file, if the
   run is stopped/paused, this parameter decides whether
   to throw exception and stop the process, or wait for
   the run to be started again. Default is False
 
   run_check_interval_s: if wait_for_run=True, this
```

### Comparing `branchkey-2.5.6/setup.py` & `branchkey-2.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(os.path.join(current_directory, "README.md"), encoding="utf-8") as f:
         long_description = f.read()
 except Exception:
     long_description = ""
 
 setuptools.setup(
     name="branchkey",
-    version="2.5.6",
+    version="2.6.0",
     author="BranchKey",
     author_email="info@branchkey.com",
     description="Client application to interface with the BranchKey system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://branchkey.com",
     project_urls={
```

### Comparing `branchkey-2.5.6/src/branchkey/__consumer.py` & `branchkey-2.6.0/src/branchkey/__consumer.py`

 * *Files identical despite different names*

### Comparing `branchkey-2.5.6/src/branchkey/client.py` & `branchkey-2.6.0/src/branchkey/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,27 @@
 from .utils import AGGREGATED_OUTPUT_DIR, FILE_METADATA
 
 
 class Client:
     def __init__(self,
                  credentials: dict = None,
                  host: str = "https://api.branchkey.com",
-                 ssl: bool = False, wait_for_run: bool = False, run_check_interval_s: int = 30):
+                 ssl: bool = True, wait_for_run: bool = False, run_check_interval_s: int = 30):
 
         if credentials is None:
             credentials = dict(leaf_name="guest", leaf_id="guest", leaf_session_token="guest",
                                response_host="response.branchkey.com", port=5672)
 
         self.__leaf_name = credentials["leaf_name"]
         self.__leaf_id = credentials["leaf_id"]
         self.__leaf_session_token = credentials["leaf_session_token"]
         self.__status = "unauthenticated"
         self.__tree_id = None
         self.__branch_id = None
 
-        self.__performance_analyser_username = credentials["performance_analyser_username"]
-        self.__performance_analyser_password = credentials["performance_analyser_password"]
-
         self.__api_host = host
         # Verify SSL certs
         self.__verify = ssl
 
         self.queue = Queue()
         self.__run_status = None
         self.__run_number = None
@@ -230,15 +227,15 @@
                                "aggregation_id": aggregation_id,
                                "leaf_id": self.__leaf_id,
                                "branch_id": self.__branch_id,
                                "tree_id": self.__tree_id,
                                "data": data})
 
             resp = requests.post(url, headers=headers, data=data,
-                                 auth=(self.__performance_analyser_username, self.__performance_analyser_password), verify=self.__verify)
+                                 auth=(self.__leaf_id, self.__leaf_session_token), verify=self.__verify)
 
             print(
                 f"received resp code form performance_analyser: {resp.status_code}")
             if resp.status_code != HTTPStatus.CREATED:
                 raise Exception(resp.json())
             else:
                 return True
```

### Comparing `branchkey-2.5.6/src/branchkey.egg-info/PKG-INFO` & `branchkey-2.6.0/src/branchkey.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: branchkey
-Version: 2.5.6
+Version: 2.6.0
 Summary: Client application to interface with the BranchKey system
 Home-page: https://branchkey.com
 Author: BranchKey
 Author-email: info@branchkey.com
 Project-URL: Homepage, https://branchkey.com
 Project-URL: Repository, https://gitlab.com/branchkey/client_application
 Classifier: Programming Language :: Python :: 3
@@ -41,25 +41,24 @@
   ```python
   import json
   from branchkey.client import Client
 
   credentials = {"leaf_name": "leaf-1",
                  "leaf_id": "46780841-9787-41e6-ac14-e3ee160e158a",
                  "leaf_session_token": "46780841-9787-41e6-ac14-e3ee160e158a",
-                 "performance_analyser_username": "hello",
-                 "performance_analyser_password": "world",
                  "response_host":"response.branchkey.com"}
 
   host = "http://api.branchkey.com"
 
   '''initialise the client
   it implicitly authenticates the leaf_session
   and fetches the run_details of the parent branch
 
-  ssl: Whether to verify the SSL certificates of the remote host or not
+  ssl: Whether to verify the SSL certificates of the
+  remote host or not. Default it True
 
   wait_for_run: When trying to upload file, if the
   run is stopped/paused, this parameter decides whether
   to throw exception and stop the process, or wait for
   the run to be started again. Default is False
 
   run_check_interval_s: if wait_for_run=True, this
```

