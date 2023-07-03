# Comparing `tmp/cq_queryabolt-0.0.1.post1.tar.gz` & `tmp/cq_queryabolt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq_queryabolt-0.0.1.post1.tar", max compression
+gzip compressed data, was "cq_queryabolt-0.0.2.tar", max compression
```

## Comparing `cq_queryabolt-0.0.1.post1.tar` & `cq_queryabolt-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3322 2023-07-02 20:14:39.033933 cq_queryabolt-0.0.1.post1/README.md
--rw-r--r--   0        0        0     3716 2023-05-24 10:11:23.149462 cq_queryabolt-0.0.1.post1/bolts.json
--rw-r--r--   0        0        0     4659 2023-07-02 20:37:29.633849 cq_queryabolt-0.0.1.post1/cq_queryabolt.py
--rw-r--r--   0        0        0     5855 2023-05-21 11:38:31.745152 cq_queryabolt-0.0.1.post1/nuts.json
--rw-r--r--   0        0        0      490 2023-07-03 10:19:33.472077 cq_queryabolt-0.0.1.post1/pyproject.toml
--rw-r--r--   0        0        0     4146 1970-01-01 00:00:00.000000 cq_queryabolt-0.0.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     3322 2023-07-02 20:14:39.033933 cq_queryabolt-0.0.2/README.md
+-rw-r--r--   0        0        0     3716 2023-05-24 10:11:23.149462 cq_queryabolt-0.0.2/bolts.json
+-rw-r--r--   0        0        0     4659 2023-07-02 20:37:29.633849 cq_queryabolt-0.0.2/cq_queryabolt.py
+-rw-r--r--   0        0        0     5855 2023-05-21 11:38:31.745152 cq_queryabolt-0.0.2/nuts.json
+-rw-r--r--   0        0        0      488 2023-07-03 10:22:25.105563 cq_queryabolt-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 cq_queryabolt-0.0.2/PKG-INFO
```

### Comparing `cq_queryabolt-0.0.1.post1/README.md` & `cq_queryabolt-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cq_queryabolt-0.0.1.post1/bolts.json` & `cq_queryabolt-0.0.2/bolts.json`

 * *Files identical despite different names*

### Comparing `cq_queryabolt-0.0.1.post1/cq_queryabolt.py` & `cq_queryabolt-0.0.2/cq_queryabolt.py`

 * *Files identical despite different names*

### Comparing `cq_queryabolt-0.0.1.post1/nuts.json` & `cq_queryabolt-0.0.2/nuts.json`

 * *Files identical despite different names*

### Comparing `cq_queryabolt-0.0.1.post1/PKG-INFO` & `cq_queryabolt-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq-queryabolt
-Version: 0.0.1.post1
+Version: 0.0.2
 Summary: A quick way to create nutcatches, screw holes and countersinks in CadQuery, according to fastener standards
 Author: Maciej Małecki
 Author-email: me@mmalecki.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

