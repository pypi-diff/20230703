# Comparing `tmp/fast-webflow-0.3.2.tar.gz` & `tmp/fast-webflow-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-webflow-0.3.2.tar", last modified: Sun Jul  2 15:43:07 2023, max compression
+gzip compressed data, was "fast-webflow-0.3.3.tar", last modified: Sun Jul  2 22:06:09 2023, max compression
```

## Comparing `fast-webflow-0.3.2.tar` & `fast-webflow-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:43:07.514972 fast-webflow-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-02 15:43:07.514972 fast-webflow-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-02 15:43:07.514972 fast-webflow-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:43:07.510972 fast-webflow-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:43:07.514972 fast-webflow-0.3.2/src/fast_webflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-02 15:43:07.000000 fast-webflow-0.3.2/src/fast_webflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 15:43:07.000000 fast-webflow-0.3.2/src/fast_webflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:43:07.000000 fast-webflow-0.3.2/src/fast_webflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 15:43:07.000000 fast-webflow-0.3.2/src/fast_webflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:43:07.514972 fast-webflow-0.3.2/src/webflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/src/webflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:43:07.514972 fast-webflow-0.3.2/src/webflow/cms/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/src/webflow/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/src/webflow/cms/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/src/webflow/cms/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/src/webflow/cms/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/src/webflow/cms/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-02 15:42:55.000000 fast-webflow-0.3.2/src/webflow/cms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 22:05:54.000000 fast-webflow-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-02 22:05:54.000000 fast-webflow-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-02 22:06:09.624115 fast-webflow-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.616115 fast-webflow-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/src/fast_webflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-02 22:06:09.000000 fast-webflow-0.3.3/src/fast_webflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 22:06:09.000000 fast-webflow-0.3.3/src/fast_webflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:06:09.000000 fast-webflow-0.3.3/src/fast_webflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 22:06:09.000000 fast-webflow-0.3.3/src/fast_webflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/src/webflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:09.620115 fast-webflow-0.3.3/src/webflow/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-02 22:05:55.000000 fast-webflow-0.3.3/src/webflow/cms/utils.py
```

### Comparing `fast-webflow-0.3.2/LICENSE` & `fast-webflow-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.3.2/PKG-INFO` & `fast-webflow-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.3.2
+Version: 0.3.3
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast-webflow-0.3.2/README.md` & `fast-webflow-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.3.2/setup.cfg` & `fast-webflow-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fast-webflow
-version = 0.3.2
+version = 0.3.3
 author = Thomas Cilloni
 author_email = tcilloni@outlook.com
 description = A client library to communicate with the WebFlow API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tcilloni/fast-webflow
 project_urls =
```

### Comparing `fast-webflow-0.3.2/src/fast_webflow.egg-info/PKG-INFO` & `fast-webflow-0.3.3/src/fast_webflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.3.2
+Version: 0.3.3
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast-webflow-0.3.2/src/webflow/cms/collection.py` & `fast-webflow-0.3.3/src/webflow/cms/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,32 +32,32 @@
                 rate limit. Defaults to 10.
             max_retries (int, optional): number of times failed requests are retried (including 
                 after hitting rate limits). Defaults to 50.
         """
         self.id = collection_id
         self.delay = throttle_delay
         self.max_retries = max_retries
-        self.data = self.get_data()
 
         self._url = f'https://api.webflow.com/collections/{collection_id}'
         self._items_url = f'https://api.webflow.com/collections/{collection_id}/items?live="true"'
         self._headers = make_headers()
         self._max_items_per_request = 100
+        self.data = self.get_data()
     
 
     def get_data(self) -> dict[str, any]:
         '''
         Fetch the collection's information.
         See the `official documentation <https://developers.webflow.com/reference/get-collection>`__ 
         for more info. Upon being called, this method will also update the object's internal dictionary.
 
         Returns:
             dict[str, any]: information about this collection (name, slug, etc.).
         '''
-        self.data = self._request(requests.get)
+        self.data = self._request(requests.get, self._url)
         return self.data
     
 
     def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict[str, any]:
         '''
         Default request method for the collection object.
 
@@ -160,16 +160,16 @@
         data = {}
 
         # split IDs into lists of max 100 items
         item_ids = [item_ids[i:i+max_items] for i in range(0, len(item_ids), max_items)]
         payloads = [{"itemIds": ids} for ids in item_ids]
 
         # send parallel requests
-        parallel_arguments = zip(repeat(self._items_url), payloads)
-        returns  = parallelize(lambda args: requests.delete(*args), parallel_arguments)
+        delete_fn = lambda data : self._request(requests.delete, self._items_url, data)
+        returns  = parallelize(delete_fn, payloads)
 
         # merge responses
         for key in ['deletedItemIds', 'errors']:
             data[key] = [item for resp in returns for item in resp[key]]
 
         return data
     
@@ -201,17 +201,17 @@
         updated number of records in the collection; then uses that number to calculate the number 
         of pages and send the requests.
 
         Returns:
             list[dict]: list of each item's data.
         '''
         # update total number of items
-        self.data = self.get_data()
         max_items = self._max_items_per_request  # API rule
-        total = self.data['total']
+        initial_data = self._request(requests.get, self._items_url)
+        total = initial_data['total']
 
         # prepare one URL request for each offset in 0..total..limit
         item_lists = parallelize(self.get_items, range(0, total, max_items))
         all_items = [item for item_list in item_lists for item in item_list['items']]
         
         return all_items
```

### Comparing `fast-webflow-0.3.2/src/webflow/cms/config.py` & `fast-webflow-0.3.3/src/webflow/cms/config.py`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.3.2/src/webflow/cms/item.py` & `fast-webflow-0.3.3/src/webflow/cms/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,30 @@
                 rate limit. Defaults to 10.
             max_retries (int, optional): number of times failed requests are retried (including 
                 after hitting rate limits). Defaults to 50.
         '''
         self.id = item_id
         self.delay = throttle_delay
         self.max_retries = max_retries
-        self.data = self.get_data()
 
-        self._url = f'https://api.webflow.com/collections/{collection_id}/items/{item_id}?live=true'
+        self._url = f'https://api.webflow.com/collections/{collection_id}/items/{item_id}'
         self._headers = make_headers()
+        self.data = self.get_data()
     
 
     def get_data(self) -> dict[str, any]:
         '''
         Fetch the item's information.
         See the `official documentation <https://developers.webflow.com/reference/get-item>`__ 
         for more info. Upon being called, this method will also update the object's internal dictionary.
 
         Returns:
             dict[str, any]: information about this item (name, slug, etc.).
         '''
-        self.data = self._request(requests.get)
+        self.data = self._request(requests.get)['items'][0]
         return self.data
     
 
     def _request(self, request_fn: callable, url: str = None, data: dict = None) -> dict[str, any]:
         '''
         Default request method for the item object.
```

### Comparing `fast-webflow-0.3.2/src/webflow/cms/site.py` & `fast-webflow-0.3.3/src/webflow/cms/site.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,18 @@
                 rate limit. Defaults to 10.
             max_retries (int, optional): number of times failed requests are retried (including 
                 after hitting rate limits). Defaults to 50.
         '''
         self.id = site_id
         self.delay = throttle_delay
         self.max_retries = max_retries
-        self.data = self.get_data()
 
         self._url = f'https://api.webflow.com/sites/{site_id}'
         self._headers = make_headers()
+        self.data = self.get_data()
     
 
     def get_data(self) -> dict[str, any]:
         '''
         Fetch the site's information.
         See the `official documentation <https://developers.webflow.com/reference/get-site>`__ 
         for more info. Upon being called, this method will also update the object's internal dictionary.
```

### Comparing `fast-webflow-0.3.2/src/webflow/cms/utils.py` & `fast-webflow-0.3.3/src/webflow/cms/utils.py`

 * *Files identical despite different names*

