# Comparing `tmp/neuralpit-2.0.1.tar.gz` & `tmp/neuralpit-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-2.0.1.tar", last modified: Sat Jul  1 20:15:32 2023, max compression
+gzip compressed data, was "neuralpit-2.0.2.tar", last modified: Mon Jul  3 13:45:00 2023, max compression
```

## Comparing `neuralpit-2.0.1.tar` & `neuralpit-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 20:15:32.202197 neuralpit-2.0.1/
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 20:14:58.000000 neuralpit-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-01 20:15:32.202197 neuralpit-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-01 20:14:58.000000 neuralpit-2.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-01 20:14:58.000000 neuralpit-2.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 20:15:32.202197 neuralpit-2.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 20:15:32.198197 neuralpit-2.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 20:15:32.202197 neuralpit-2.0.1/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      586 2023-07-01 20:14:58.000000 neuralpit-2.0.1/src/neuralpit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 20:15:32.202197 neuralpit-2.0.1/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-01 20:14:58.000000 neuralpit-2.0.1/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-07-01 20:14:58.000000 neuralpit-2.0.1/src/neuralpit/services/conversation.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-01 20:14:58.000000 neuralpit-2.0.1/src/neuralpit/services/conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 20:15:32.202197 neuralpit-2.0.1/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-01 20:15:32.000000 neuralpit-2.0.1/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-01 20:15:32.000000 neuralpit-2.0.1/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 20:15:32.000000 neuralpit-2.0.1/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-01 20:15:32.000000 neuralpit-2.0.1/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-01 20:15:32.000000 neuralpit-2.0.1/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 20:15:32.202197 neuralpit-2.0.1/test/
--rw-r--r--   0 root         (0) root         (0)      411 2023-07-01 20:14:58.000000 neuralpit-2.0.1/test/testCreateConversation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:45:00.563739 neuralpit-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 13:44:30.000000 neuralpit-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-03 13:45:00.563739 neuralpit-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-03 13:44:30.000000 neuralpit-2.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-03 13:44:30.000000 neuralpit-2.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 13:45:00.563739 neuralpit-2.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:45:00.559739 neuralpit-2.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:45:00.563739 neuralpit-2.0.2/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-03 13:44:30.000000 neuralpit-2.0.2/src/neuralpit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:45:00.563739 neuralpit-2.0.2/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 13:44:30.000000 neuralpit-2.0.2/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-07-03 13:44:30.000000 neuralpit-2.0.2/src/neuralpit/services/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-03 13:44:30.000000 neuralpit-2.0.2/src/neuralpit/services/conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:45:00.563739 neuralpit-2.0.2/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-03 13:45:00.000000 neuralpit-2.0.2/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-03 13:45:00.000000 neuralpit-2.0.2/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 13:45:00.000000 neuralpit-2.0.2/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-03 13:45:00.000000 neuralpit-2.0.2/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-03 13:45:00.000000 neuralpit-2.0.2/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 13:45:00.563739 neuralpit-2.0.2/test/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-07-03 13:44:30.000000 neuralpit-2.0.2/test/testCreateConversation.py
```

### Comparing `neuralpit-2.0.1/PKG-INFO` & `neuralpit-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.0.1
+Version: 2.0.2
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-2.0.1/pyproject.toml` & `neuralpit-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "2.0.1"
+version = "2.0.2"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-2.0.1/src/neuralpit/__init__.py` & `neuralpit-2.0.2/src/neuralpit/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.0.1/src/neuralpit/services/conversation.py` & `neuralpit-2.0.2/src/neuralpit/services/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,8 +63,14 @@
         return resp
     
     def queryConversation(self, conversation_id, question):
         post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/query')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
         post_call = requests.post(post_url, headers = headers, json = {'question': question})
         resp =  json.loads(post_call.content)
-        return resp
+        return resp
+    
+    def summarizeDocument(self, conversation_id, document_id):
+        post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/document/{document_id}/summarize')
+        headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
+        post_call = requests.post(post_url, headers = headers)
+        return post_call.content
```

### Comparing `neuralpit-2.0.1/src/neuralpit/services/conversion.py` & `neuralpit-2.0.2/src/neuralpit/services/conversion.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.0.1/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-2.0.2/src/neuralpit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.0.1
+Version: 2.0.2
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

