# Comparing `tmp/citybrain-official-0.6.tar.gz` & `tmp/citybrain-official-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citybrain-official-0.6.tar", last modified: Mon Jul  3 07:39:51 2023, max compression
+gzip compressed data, was "citybrain-official-0.7.tar", last modified: Mon Jul  3 09:00:01 2023, max compression
```

## Comparing `citybrain-official-0.6.tar` & `citybrain-official-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-03 07:39:51.776167 citybrain-official-0.6/
--rw-r--r--   0 mabingtao   (501) staff       (20)     1060 2023-07-02 14:17:08.000000 citybrain-official-0.6/LICENSE
--rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-03 07:39:51.775599 citybrain-official-0.6/PKG-INFO
--rw-r--r--   0 mabingtao   (501) staff       (20)      802 2023-07-03 07:35:48.000000 citybrain-official-0.6/README.md
-drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-03 07:39:51.774194 citybrain-official-0.6/citybrain_official/
--rw-r--r--   0 mabingtao   (501) staff       (20)       88 2023-07-03 07:13:50.000000 citybrain-official-0.6/citybrain_official/__init__.py
--rw-r--r--   0 mabingtao   (501) staff       (20)     4759 2023-07-03 07:27:29.000000 citybrain-official-0.6/citybrain_official/client.py
-drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-03 07:39:51.775358 citybrain-official-0.6/citybrain_official.egg-info/
--rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-03 07:39:51.000000 citybrain-official-0.6/citybrain_official.egg-info/PKG-INFO
--rw-r--r--   0 mabingtao   (501) staff       (20)      295 2023-07-03 07:39:51.000000 citybrain-official-0.6/citybrain_official.egg-info/SOURCES.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)        1 2023-07-03 07:39:51.000000 citybrain-official-0.6/citybrain_official.egg-info/dependency_links.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)       16 2023-07-03 07:39:51.000000 citybrain-official-0.6/citybrain_official.egg-info/requires.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)       19 2023-07-03 07:39:51.000000 citybrain-official-0.6/citybrain_official.egg-info/top_level.txt
--rw-r--r--   0 mabingtao   (501) staff       (20)       38 2023-07-03 07:39:51.776236 citybrain-official-0.6/setup.cfg
--rw-r--r--   0 mabingtao   (501) staff       (20)      673 2023-07-03 07:39:38.000000 citybrain-official-0.6/setup.py
+drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-03 09:00:01.087763 citybrain-official-0.7/
+-rw-r--r--   0 mabingtao   (501) staff       (20)     1060 2023-07-02 14:17:08.000000 citybrain-official-0.7/LICENSE
+-rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-03 09:00:01.087552 citybrain-official-0.7/PKG-INFO
+-rw-r--r--   0 mabingtao   (501) staff       (20)      802 2023-07-03 07:35:48.000000 citybrain-official-0.7/README.md
+drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-03 09:00:01.086265 citybrain-official-0.7/citybrain_official/
+-rw-r--r--   0 mabingtao   (501) staff       (20)       88 2023-07-03 07:13:50.000000 citybrain-official-0.7/citybrain_official/__init__.py
+-rw-r--r--   0 mabingtao   (501) staff       (20)     5480 2023-07-03 08:59:12.000000 citybrain-official-0.7/citybrain_official/client.py
+drwxr-xr-x   0 mabingtao   (501) staff       (20)        0 2023-07-03 09:00:01.087261 citybrain-official-0.7/citybrain_official.egg-info/
+-rw-r--r--   0 mabingtao   (501) staff       (20)     1251 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/PKG-INFO
+-rw-r--r--   0 mabingtao   (501) staff       (20)      295 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/SOURCES.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)        1 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/dependency_links.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)       16 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/requires.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)       19 2023-07-03 09:00:01.000000 citybrain-official-0.7/citybrain_official.egg-info/top_level.txt
+-rw-r--r--   0 mabingtao   (501) staff       (20)       38 2023-07-03 09:00:01.087826 citybrain-official-0.7/setup.cfg
+-rw-r--r--   0 mabingtao   (501) staff       (20)      673 2023-07-03 08:59:47.000000 citybrain-official-0.7/setup.py
```

### Comparing `citybrain-official-0.6/LICENSE` & `citybrain-official-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `citybrain-official-0.6/PKG-INFO` & `citybrain-official-0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citybrain-official
-Version: 0.6
+Version: 0.7
 Summary: retrieve data from citybrain.org
 Home-page: UNKNOWN
 Author: citybrain.org
 Author-email: opensource@citybrain.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citybrain-official-0.6/README.md` & `citybrain-official-0.7/README.md`

 * *Files identical despite different names*

### Comparing `citybrain-official-0.6/citybrain_official/client.py` & `citybrain-official-0.7/citybrain_official/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,112 +1,134 @@
 import requests
 import json
 import os
+import csv
+import time
+from io import StringIO
 import pandas
 
 __DEFAULT_ENDPOINT = "https://dev.citybrain.org/api/getData"
 __DEFAULT_ODPS_DATA_ADDRESS = "170DD61338021000"
 
 endpoint: str = ""
 
 def __get_endpoint() -> str:
-    if endpoint != "":
+    if endpoint != '':
         return endpoint
     envEndpoint = os.getenv('ENDPOINT')
-    if envEndpoint is not None and envEndpoint != "":
+    if envEndpoint is not None and envEndpoint != '':
         return envEndpoint
     return __DEFAULT_ENDPOINT
 
 
 def __get_odps_dataaddress(dataAddress: str) -> str:
-    if dataAddress != "":
+    if dataAddress != '':
         return dataAddress
     envODPSDataAddress = os.getenv('ODPS_DATA_ADDRESS')
-    if envODPSDataAddress is not None and envODPSDataAddress != "":
+    if envODPSDataAddress is not None and envODPSDataAddress != '':
         return envODPSDataAddress
     return __DEFAULT_ODPS_DATA_ADDRESS
 
-def retrieve_raw(dataAddress: str, sql: str) -> any:
-    if sql is None or sql == '':
-        return __download_csv(dataAddress=dataAddress)
+def retrieve_raw(dataAddress: str = '', sql: str = '') -> any:
+    if sql == '':
+        if dataAddress == '':
+            raise Exception('must specify data address')
+        content = __download_file(dataAddress=dataAddress)
+        return content.replace('\ufeff', '', 1)
     else:
         # create odps sql task
-        taskID = createSQLTask(dataAddress=dataAddress, sql=sql)
+        taskID = __create_sql_task(dataAddress=dataAddress, sql=sql)
 
         # query task status until terminated
-        status = queryTaskStatus(dataAddress=dataAddress, taskID=taskID)
+        status = __query_task_status(dataAddress=dataAddress, taskID=taskID)
         while status != 'Terminated':
-            status = queryTaskStatus(dataAddress=dataAddress, taskID=taskID)
+            time.sleep(2)
+            status = __query_task_status(dataAddress=dataAddress, taskID=taskID)
 
         # download task result
         return __download_task_result(dataAddress=dataAddress, taskID=taskID)
 
-def retrieve_df(dataAddress: str, sql: str) -> pandas.DataFrame:
-    if sql is None or sql == '':
-        csvData = __download_csv(dataAddress=dataAddress)
-        return __parse_list_to_dataframe(csvData)
-    else:
+def retrieve_df(dataAddress: str = '', sql: str = '') -> pandas.DataFrame:
+    if sql == '': # file data
+        if dataAddress == '':
+            raise Exception('must specify data address')
+        # download file content
+        content = __download_file(dataAddress=dataAddress)
+        content = content.replace('\ufeff', '', 1)
+
+        # convert to dataframe
+        src = []
+        tmp = StringIO(content)
+        csvReader = csv.reader(tmp, delimiter=',')
+        for row in csvReader:
+            src.append(row)
+        return pandas.DataFrame(src[1:], columns=src[0])
+        
+    else: # odps data
         # create odps sql task
-        taskID = createSQLTask(dataAddress=dataAddress, sql=sql)
+        taskID = __create_sql_task(dataAddress=dataAddress, sql=sql)
 
         # query task status until terminated
-        status = queryTaskStatus(dataAddress=dataAddress, taskID=taskID)
+        status = __query_task_status(dataAddress=dataAddress, taskID=taskID)
         while status != 'Terminated':
-            status = queryTaskStatus(dataAddress=dataAddress, taskID=taskID)
+            time.sleep(2)
+            status = __query_task_status(dataAddress=dataAddress, taskID=taskID)
 
         # download task result
         result = __download_task_result(dataAddress=dataAddress, taskID=taskID)
-        return __parse_list_to_dataframe(result)
+
+        # convert to dataframe
+        if len(result) == 0:
+            return pandas.DataFrame([])
+        src = []
+        for row in result[1:]:
+            src.append(row.split(';'))
+        return pandas.DataFrame(src, columns=result[0].split(';'))
     
-def __download_csv(dataAddress: str) -> list[str]:
+def __download_file(dataAddress: str) -> str:
     endpoint = __get_endpoint()
     reqBody = {'dpAddress': dataAddress, 'payload': ''}
     resp = requests.post(url=endpoint, headers={'content-type': 'application/json'}, json=reqBody, timeout=None)
     if resp.status_code != 200:
         raise Exception('request failed, status code is: ' + str(resp.status_code))
     result = resp.json()
     if result['code'] != 200:
         raise Exception('server error: message is: ' + str(result['message']))
     if isinstance(result['data'], str):
-        return result['data'].split('\n')
+        return result['data']
 
-def __parse_list_to_dataframe(rows: list[str]) -> pandas.DataFrame:
-    if len(rows) == 0:
-        return pandas.DataFrame([])
-    src = []
-    for row in rows[1:]:
-        src.append(row.split(';'))
-    return pandas.DataFrame(src, columns=rows[0].split(';'))
 	
 def __download_task_result(dataAddress: str, taskID: str) -> list[str]:
     endpoint = __get_endpoint()
+    dataAddress = __get_odps_dataaddress(dataAddress=dataAddress)
     reqBody = {"dpAddress": dataAddress, 'payload': json.dumps({'payload': taskID, 'action': 'TASK_DownloadResult'})}
     resp = requests.post(url=endpoint, headers={'content-type': 'application/json'}, json=reqBody, timeout=None)
     if resp.status_code != 200:
         raise Exception('request failed, status code is: ' + str(resp.status_code))
     result = resp.json()
     if result['code'] != 200:
         raise Exception('server error: message is: ' + str(result['message']))
     strList = json.loads(result['data'])
     return strList
 
 
-def queryTaskStatus(dataAddress: str, taskID: str) -> str:
+def __query_task_status(dataAddress: str, taskID: str) -> str:
     endpoint = __get_endpoint()
+    dataAddress = __get_odps_dataaddress(dataAddress=dataAddress)
     reqBody = {"dpAddress": dataAddress, 'payload': json.dumps({'payload': taskID, 'action': 'TASK_QueryStatus'})}
     resp = requests.post(url=endpoint, headers={'content-type': 'application/json'}, json=reqBody, timeout=None)
     if resp.status_code != 200:
         raise Exception('request failed, status code is: ' + str(resp.status_code))
     result = resp.json()
     if result['code'] != 200:
         raise Exception('server error: message is: ' + str(result['message']))
     return result['data']
 
 
-def createSQLTask(dataAddress: str, sql: str) -> str:
+def __create_sql_task(dataAddress: str, sql: str) -> str:
     endpoint = __get_endpoint()
     dataAddress = __get_odps_dataaddress(dataAddress=dataAddress)
     reqBody = {'dpAddress': dataAddress,'payload': json.dumps({'payload': sql, 'action':'TASK_Create'})}
     resp = requests.post(url=endpoint, headers={'content-type': 'application/json'}, json=reqBody, timeout=None)
     if resp.status_code != 200:
         raise Exception('request failed, status code is: ' + str(resp.status_code))
     result = resp.json()
```

### Comparing `citybrain-official-0.6/citybrain_official.egg-info/PKG-INFO` & `citybrain-official-0.7/citybrain_official.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citybrain-official
-Version: 0.6
+Version: 0.7
 Summary: retrieve data from citybrain.org
 Home-page: UNKNOWN
 Author: citybrain.org
 Author-email: opensource@citybrain.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `citybrain-official-0.6/setup.py` & `citybrain-official-0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="citybrain-official",
-    version="0.6",
+    version="0.7",
     author="citybrain.org",
     author_email="opensource@citybrain.org",
     description="retrieve data from citybrain.org",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

