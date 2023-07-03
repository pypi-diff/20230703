# Comparing `tmp/pGerrit-0.1.5.tar.gz` & `tmp/pGerrit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pGerrit-0.1.5.tar", last modified: Wed May 17 11:51:53 2023, max compression
+gzip compressed data, was "pGerrit-0.1.6.tar", last modified: Mon Jul  3 07:06:53 2023, max compression
```

## Comparing `pGerrit-0.1.5.tar` & `pGerrit-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-05-17 11:51:53.325699 pGerrit-0.1.5/
--rw-rw-r--   0 cy        (1000) cy        (1000)      891 2023-05-17 11:51:53.325699 pGerrit-0.1.5/PKG-INFO
--rw-rw-r--   0 cy        (1000) cy        (1000)     3288 2023-05-17 06:38:32.000000 pGerrit-0.1.5/README.md
-drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-05-17 11:51:53.325699 pGerrit-0.1.5/pGerrit/
--rw-rw-r--   0 cy        (1000) cy        (1000)     1431 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/Access.py
--rw-rw-r--   0 cy        (1000) cy        (1000)      987 2023-04-04 12:31:47.000000 pGerrit-0.1.5/pGerrit/ApprovalInfo.py
--rw-rw-r--   0 cy        (1000) cy        (1000)       21 2023-05-17 11:48:49.000000 pGerrit-0.1.5/pGerrit/__init__.py
--rw-rw-r--   0 cy        (1000) cy        (1000)    35397 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/change.py
--rw-rw-r--   0 cy        (1000) cy        (1000)     4033 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/client.py
--rw-rw-r--   0 cy        (1000) cy        (1000)     2292 2023-05-17 11:48:26.000000 pGerrit-0.1.5/pGerrit/project.py
--rw-rw-r--   0 cy        (1000) cy        (1000)     3859 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/queryDescriptor.py
--rw-rw-r--   0 cy        (1000) cy        (1000)     3778 2023-05-17 06:38:32.000000 pGerrit-0.1.5/pGerrit/restAPIwrapper.py
--rw-rw-r--   0 cy        (1000) cy        (1000)      772 2023-03-31 11:18:07.000000 pGerrit-0.1.5/pGerrit/utils.py
-drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-05-17 11:51:53.325699 pGerrit-0.1.5/pGerrit.egg-info/
--rw-rw-r--   0 cy        (1000) cy        (1000)      891 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/PKG-INFO
--rw-rw-r--   0 cy        (1000) cy        (1000)      401 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/SOURCES.txt
--rw-rw-r--   0 cy        (1000) cy        (1000)        1 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/dependency_links.txt
--rw-rw-r--   0 cy        (1000) cy        (1000)       24 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/requires.txt
--rw-rw-r--   0 cy        (1000) cy        (1000)       14 2023-05-17 11:51:53.000000 pGerrit-0.1.5/pGerrit.egg-info/top_level.txt
--rw-rw-r--   0 cy        (1000) cy        (1000)      847 2023-05-17 11:51:53.325699 pGerrit-0.1.5/setup.cfg
--rw-rw-r--   0 cy        (1000) cy        (1000)       68 2023-03-31 11:18:07.000000 pGerrit-0.1.5/setup.py
-drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-05-17 11:51:53.325699 pGerrit-0.1.5/tests/
--rw-rw-r--   0 cy        (1000) cy        (1000)        0 2023-03-29 03:40:33.000000 pGerrit-0.1.5/tests/__init__.py
--rw-rw-r--   0 cy        (1000) cy        (1000)    13790 2023-05-17 06:38:32.000000 pGerrit-0.1.5/tests/test.py
+drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-07-03 07:06:53.566140 pGerrit-0.1.6/
+-rw-rw-r--   0 cy        (1000) cy        (1000)      891 2023-07-03 07:06:53.566140 pGerrit-0.1.6/PKG-INFO
+-rw-rw-r--   0 cy        (1000) cy        (1000)     3288 2023-05-17 06:38:32.000000 pGerrit-0.1.6/README.md
+drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-07-03 07:06:53.566140 pGerrit-0.1.6/pGerrit/
+-rw-rw-r--   0 cy        (1000) cy        (1000)     1431 2023-05-17 06:38:32.000000 pGerrit-0.1.6/pGerrit/Access.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)       21 2023-07-03 07:05:33.000000 pGerrit-0.1.6/pGerrit/__init__.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)    36085 2023-06-30 09:02:26.000000 pGerrit-0.1.6/pGerrit/change.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)     4033 2023-05-17 06:38:32.000000 pGerrit-0.1.6/pGerrit/client.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)     2292 2023-05-17 11:48:26.000000 pGerrit-0.1.6/pGerrit/project.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)     3859 2023-05-17 06:38:32.000000 pGerrit-0.1.6/pGerrit/queryDescriptor.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)     3778 2023-05-17 06:38:32.000000 pGerrit-0.1.6/pGerrit/restAPIwrapper.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)      772 2023-03-31 11:18:07.000000 pGerrit-0.1.6/pGerrit/utils.py
+drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-07-03 07:06:53.566140 pGerrit-0.1.6/pGerrit.egg-info/
+-rw-rw-r--   0 cy        (1000) cy        (1000)      891 2023-07-03 07:06:53.000000 pGerrit-0.1.6/pGerrit.egg-info/PKG-INFO
+-rw-rw-r--   0 cy        (1000) cy        (1000)      377 2023-07-03 07:06:53.000000 pGerrit-0.1.6/pGerrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 cy        (1000) cy        (1000)        1 2023-07-03 07:06:53.000000 pGerrit-0.1.6/pGerrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 cy        (1000) cy        (1000)       24 2023-07-03 07:06:53.000000 pGerrit-0.1.6/pGerrit.egg-info/requires.txt
+-rw-rw-r--   0 cy        (1000) cy        (1000)       14 2023-07-03 07:06:53.000000 pGerrit-0.1.6/pGerrit.egg-info/top_level.txt
+-rw-rw-r--   0 cy        (1000) cy        (1000)      847 2023-07-03 07:06:53.566140 pGerrit-0.1.6/setup.cfg
+-rw-rw-r--   0 cy        (1000) cy        (1000)       68 2023-03-31 11:18:07.000000 pGerrit-0.1.6/setup.py
+drwxrwxr-x   0 cy        (1000) cy        (1000)        0 2023-07-03 07:06:53.566140 pGerrit-0.1.6/tests/
+-rw-rw-r--   0 cy        (1000) cy        (1000)        0 2023-03-29 03:40:33.000000 pGerrit-0.1.6/tests/__init__.py
+-rw-rw-r--   0 cy        (1000) cy        (1000)    14092 2023-06-30 08:43:44.000000 pGerrit-0.1.6/tests/test.py
```

### Comparing `pGerrit-0.1.5/PKG-INFO` & `pGerrit-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pGerrit
-Version: 0.1.5
+Version: 0.1.6
 Summary: A well designed base on decorator pattern library to access Google Gerrit REST API
 Home-page: UNKNOWN
 Author: CY
 Author-email: 17103513@qq.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/demonguy/pGerrit
 Project-URL: Tracker, https://github.com/demonguy/pGerrit/issues
```

### Comparing `pGerrit-0.1.5/README.md` & `pGerrit-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.5/pGerrit/Access.py` & `pGerrit-0.1.6/pGerrit/Access.py`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.5/pGerrit/change.py` & `pGerrit-0.1.6/pGerrit/change.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,14 +295,32 @@
         Usage::
 
             change.rebase()
 
         """
         pass
 
+    @GerritRest.post
+    @GerritRest.url_wrapper()
+    def merge(self, payload=None, headers=None):
+        """Performs a POST request to create merge patch set for change.
+
+        **API URL**: `/a/changes/{change_id}/merge <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#create-merge-patch-set-for-change>`__
+
+        **Input type**: `MergePatchSetInput <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#merge-patch-set-input>`__
+
+        **Return type**: `ChangeInfo <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#change-info>`__
+
+        Usage::
+
+            change.merge()
+
+        """
+        pass
+
     @GerritRest.delete
     @GerritRest.url_wrapper("")
     def delete_change(self, payload=None, headers=None):
         """Performs a DELETE request to delete a change.
 
         **API URL**: `/a/changes/{change_id} <https://gerrit-review.googlesource.com/Documentation/rest-api-changes.html#delete-change>`__
```

### Comparing `pGerrit-0.1.5/pGerrit/client.py` & `pGerrit-0.1.6/pGerrit/client.py`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.5/pGerrit/project.py` & `pGerrit-0.1.6/pGerrit/project.py`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.5/pGerrit/queryDescriptor.py` & `pGerrit-0.1.6/pGerrit/queryDescriptor.py`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.5/pGerrit/restAPIwrapper.py` & `pGerrit-0.1.6/pGerrit/restAPIwrapper.py`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.5/pGerrit/utils.py` & `pGerrit-0.1.6/pGerrit/utils.py`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.5/pGerrit.egg-info/PKG-INFO` & `pGerrit-0.1.6/pGerrit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pGerrit
-Version: 0.1.5
+Version: 0.1.6
 Summary: A well designed base on decorator pattern library to access Google Gerrit REST API
 Home-page: UNKNOWN
 Author: CY
 Author-email: 17103513@qq.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/demonguy/pGerrit
 Project-URL: Tracker, https://github.com/demonguy/pGerrit/issues
```

### Comparing `pGerrit-0.1.5/setup.cfg` & `pGerrit-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pGerrit-0.1.5/tests/test.py` & `pGerrit-0.1.6/tests/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,23 @@
         self.assertEqual(set(hashtags), set(target_hashtags))
 
     @unittest.skip("This change cannot be rebased, so skip")
     def testChangeRebase(self):
         rebase = self.change.rebase()
         # self.assertIsInstance(edit, SimpleNamespace)
 
+    def testChangeCreateMerge(self):
+        createMerge = self.change.merge(payload={
+            "merge": {
+                "source": self.change.revision("1").commit().commit,
+                "allow_conflicts": "True"
+            }
+        })
+        self.assertEqual(createMerge.status_code, 200)
+
     def testChangeIsMerge(self):
         self.assertTrue(self.change.is_merge())
 
     def testChangeCurrentRevision(self):
         revision = self.change.current_revision()
         self.assertIsInstance(revision, GerritChangeRevision)
```

