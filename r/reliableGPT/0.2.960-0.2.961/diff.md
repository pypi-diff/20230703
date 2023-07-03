# Comparing `tmp/reliableGPT-0.2.960.tar.gz` & `tmp/reliableGPT-0.2.961.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.960.tar", last modified: Mon Jul  3 15:33:33 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.961.tar", last modified: Mon Jul  3 15:37:48 2023, max compression
```

## Comparing `reliableGPT-0.2.960.tar` & `reliableGPT-0.2.961.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:33:33.298866 reliableGPT-0.2.960/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.960/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-03 15:33:33.298694 reliableGPT-0.2.960/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     8271 2023-07-03 15:14:41.000000 reliableGPT-0.2.960/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.960/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:33:33.295309 reliableGPT-0.2.960/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-03 15:33:33.000000 reliableGPT-0.2.960/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      514 2023-07-03 15:33:33.000000 reliableGPT-0.2.960/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-03 15:33:33.000000 reliableGPT-0.2.960/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-07-03 15:33:33.000000 reliableGPT-0.2.960/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-03 15:33:33.000000 reliableGPT-0.2.960/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:33:33.297598 reliableGPT-0.2.960/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.960/reliablegpt/APICallHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3120 2023-07-02 04:13:32.000000 reliableGPT-0.2.960/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.960/reliablegpt/CustomQueue.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11549 2023-07-03 15:14:41.000000 reliableGPT-0.2.960/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.960/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5170 2023-07-03 15:14:41.000000 reliableGPT-0.2.960/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     7119 2023-07-03 15:14:41.000000 reliableGPT-0.2.960/reliablegpt/ReliableDataLoaders.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      422 2023-07-03 15:31:25.000000 reliableGPT-0.2.960/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3900 2023-07-03 15:26:34.000000 reliableGPT-0.2.960/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.960/reliablegpt/reliableQuery.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-03 15:33:33.299292 reliableGPT-0.2.960/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      398 2023-07-03 15:31:37.000000 reliableGPT-0.2.960/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:37:48.977841 reliableGPT-0.2.961/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.961/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-03 15:37:48.977720 reliableGPT-0.2.961/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     8271 2023-07-03 15:14:41.000000 reliableGPT-0.2.961/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.961/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:37:48.975451 reliableGPT-0.2.961/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-03 15:37:48.000000 reliableGPT-0.2.961/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      514 2023-07-03 15:37:48.000000 reliableGPT-0.2.961/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-03 15:37:48.000000 reliableGPT-0.2.961/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-07-03 15:37:48.000000 reliableGPT-0.2.961/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-03 15:37:48.000000 reliableGPT-0.2.961/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-03 15:37:48.977520 reliableGPT-0.2.961/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.961/reliablegpt/APICallHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3120 2023-07-02 04:13:32.000000 reliableGPT-0.2.961/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.961/reliablegpt/CustomQueue.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11549 2023-07-03 15:14:41.000000 reliableGPT-0.2.961/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.961/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5170 2023-07-03 15:14:41.000000 reliableGPT-0.2.961/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     7119 2023-07-03 15:14:41.000000 reliableGPT-0.2.961/reliablegpt/ReliableDataLoaders.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      427 2023-07-03 15:37:38.000000 reliableGPT-0.2.961/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3900 2023-07-03 15:26:34.000000 reliableGPT-0.2.961/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2363 2023-07-03 15:14:41.000000 reliableGPT-0.2.961/reliablegpt/reliableQuery.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-03 15:37:48.977885 reliableGPT-0.2.961/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      398 2023-07-03 15:37:46.000000 reliableGPT-0.2.961/setup.py
```

### Comparing `reliableGPT-0.2.960/LICENSE` & `reliableGPT-0.2.961/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/README.md` & `reliableGPT-0.2.961/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliableGPT.egg-info/SOURCES.txt` & `reliableGPT-0.2.961/reliableGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.961/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliablegpt/Alerting.py` & `reliableGPT-0.2.961/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.961/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.961/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliablegpt/Model.py` & `reliableGPT-0.2.961/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.961/reliablegpt/RateLimitHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliablegpt/ReliableDataLoaders.py` & `reliableGPT-0.2.961/reliablegpt/ReliableDataLoaders.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliablegpt/main.py` & `reliableGPT-0.2.961/reliablegpt/main.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.960/reliablegpt/reliableQuery.py` & `reliableGPT-0.2.961/reliablegpt/reliableQuery.py`

 * *Files identical despite different names*

