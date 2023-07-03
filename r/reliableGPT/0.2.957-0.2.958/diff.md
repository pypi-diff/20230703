# Comparing `tmp/reliableGPT-0.2.957.tar.gz` & `tmp/reliableGPT-0.2.958.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.957.tar", last modified: Sun Jul  2 04:14:13 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.958.tar", last modified: Mon Jul  3 15:24:36 2023, max compression
```

## Comparing `reliableGPT-0.2.957.tar` & `reliableGPT-0.2.958.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-02 04:14:13.458633 reliableGPT-0.2.957/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.957/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-02 04:14:13.458511 reliableGPT-0.2.957/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     6254 2023-07-01 20:41:40.000000 reliableGPT-0.2.957/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.957/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-02 04:14:13.457103 reliableGPT-0.2.957/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      485 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-02 04:14:13.458323 reliableGPT-0.2.957/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.957/reliablegpt/APICallHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3120 2023-07-02 04:13:32.000000 reliableGPT-0.2.957/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.957/reliablegpt/CustomQueue.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11224 2023-07-01 20:41:40.000000 reliableGPT-0.2.957/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.957/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5195 2023-07-01 20:41:27.000000 reliableGPT-0.2.957/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     7119 2023-07-02 04:12:52.000000 reliableGPT-0.2.957/reliablegpt/ReliableDataLoaders.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      374 2023-07-01 20:43:51.000000 reliableGPT-0.2.957/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3921 2023-07-01 20:41:40.000000 reliableGPT-0.2.957/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-02 04:14:13.458673 reliableGPT-0.2.957/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      398 2023-07-02 04:14:03.000000 reliableGPT-0.2.957/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:24:36.021074 reliableGPT-0.2.958/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.958/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-03 15:24:36.020922 reliableGPT-0.2.958/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8271 2023-07-03 15:14:41.000000 reliableGPT-0.2.958/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.958/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:24:36.017543 reliableGPT-0.2.958/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-03 15:24:35.000000 reliableGPT-0.2.958/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      514 2023-07-03 15:24:35.000000 reliableGPT-0.2.958/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-03 15:24:35.000000 reliableGPT-0.2.958/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-07-03 15:24:35.000000 reliableGPT-0.2.958/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-03 15:24:35.000000 reliableGPT-0.2.958/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:24:36.020626 reliableGPT-0.2.958/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.958/reliablegpt/APICallHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3120 2023-07-02 04:13:32.000000 reliableGPT-0.2.958/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.958/reliablegpt/CustomQueue.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11549 2023-07-03 15:14:41.000000 reliableGPT-0.2.958/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.958/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5170 2023-07-03 15:14:41.000000 reliableGPT-0.2.958/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     7119 2023-07-03 15:14:41.000000 reliableGPT-0.2.958/reliablegpt/ReliableDataLoaders.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      416 2023-07-03 15:24:11.000000 reliableGPT-0.2.958/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3900 2023-07-03 15:24:05.000000 reliableGPT-0.2.958/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.958/reliablegpt/reliableQuery.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-03 15:24:36.021135 reliableGPT-0.2.958/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      398 2023-07-03 15:24:29.000000 reliableGPT-0.2.958/setup.py
```

### Comparing `reliableGPT-0.2.957/LICENSE` & `reliableGPT-0.2.958/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.957/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.958/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.957/reliablegpt/Alerting.py` & `reliableGPT-0.2.958/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.957/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.958/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.957/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.958/reliablegpt/IndividualRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import copy
 import posthog
 import importlib
 import openai
 from openai import ChatCompletion
 import traceback
 
+
 class IndividualRequest:
   """A brief description of the class."""
 
   def __init__(self,
                model=None,
                fallback_strategy=[
                  'gpt-3.5-turbo', 'text-davinci-003', 'gpt-4',
@@ -42,14 +43,23 @@
 
   ## Code that handles / wraps openai calls
   def __call__(self, *args, **kwargs):
     try:
       self.print_verbose(f"calling model function: {self.model_function}")
       self.print_verbose(f"these are the kwargs: {kwargs}")
       self.print_verbose(f"this is the openai api base: {openai.api_base}")
+      try:
+        # this should never block running the openai call
+        self.save_request(
+            user_email=self.user_email,
+            graceful_string=self.graceful_string,
+            posthog_event='reliableGPT.request',
+        )
+      except:
+        print("ReliableGPT error occured during saving request")
       result = self.model_function(*args, **kwargs)
       self.print_verbose(f"This is the result: {str(result)[:500]}")
       return result
     except Exception as e:
       self.print_verbose("catches the error")
       return self.handle_exception(args, kwargs, e)
```

### Comparing `reliableGPT-0.2.957/reliablegpt/Model.py` & `reliableGPT-0.2.958/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.957/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.958/reliablegpt/RateLimitHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import uuid
 import time
 import traceback
 
 
 ## Dev Imports 
 # from IndividualRequest import IndividualRequest
-# from RateLimitHandler_helpers.APICallHandler import APICallHandler
+# from APICallHandler import APICallHandler
 
 ## Prod Imports
 from reliablegpt.IndividualRequest import IndividualRequest
 from reliablegpt.APICallHandler import APICallHandler
 
 
 class RateLimitHandler:
```

### Comparing `reliableGPT-0.2.957/reliablegpt/ReliableDataLoaders.py` & `reliableGPT-0.2.958/reliablegpt/ReliableDataLoaders.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.957/reliablegpt/main.py` & `reliableGPT-0.2.958/reliablegpt/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # # Prod Imports
 from reliablegpt.IndividualRequest import IndividualRequest
 from reliablegpt.RateLimitHandler import RateLimitHandler
 from reliablegpt.Model import Model
-from reliablegpt.Alerting import Alerting
+from reliablegpt.alerting import Alerting
 
 # # Dev Imports
 # from IndividualRequest import IndividualRequest
 # from RateLimitHandler import RateLimitHandler
 # from Model import Model
-# from Alerting import Alerting
+# from alerting import Alerting
 
 from posthog import Posthog
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
@@ -22,15 +22,14 @@
 def save_request(user_email,
                  graceful_string,
                  posthog_event="",
                  result="",
                  posthog_metadata={},
                  errors=[]):
   try:
-    #metadata  = kwargs['metadata']
     if posthog_event != "":
       posthog.capture(user_email, posthog_event,
                       posthog_metadata)  # save posthog event
     if result == graceful_string or len(
         errors) == 2:  # returns a graceful string or got a 2nd exception
       # send an email and alert
       for error in errors:
@@ -80,17 +79,17 @@
                              backup_openai_key=backup_openai_key, 
                              verbose=verbose)
   elif queue_requests == True:
     max_token_capacity = 40000
     max_request_capacity = 200
     ## [TODO]: Allow handling multiple model types (gpt-3.5-turbo AND gpt-4)
     if model_limits_dir and isinstance(model_limits_dir, dict):
-      keys = model_limits_dir.keys()
+      keys = list(model_limits_dir.keys())
       max_token_capacity = model_limits_dir[keys[0]]["max_token_capacity"]
-      max_request_capacity = model_limits_dir["max_request_capacity"]
+      max_request_capacity = model_limits_dir[keys[0]]["max_request_capacity"]
 
     return RateLimitHandler(model,
                             fallback_strategy=fallback_strategy,
                             graceful_string=graceful_string,
                             user_email=primary_email,
                             user_token=user_token,
                             send_notification=send_notification,
```

