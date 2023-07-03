# Comparing `tmp/huhangkai-1.4.7.tar.gz` & `tmp/huhangkai-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\huhangkai-1.4.7.tar", last modified: Mon Jul  3 16:37:31 2023, max compression
+gzip compressed data, was "dist\huhangkai-1.4.8.tar", last modified: Mon Jul  3 16:38:23 2023, max compression
```

## Comparing `huhangkai-1.4.7.tar` & `huhangkai-1.4.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 16:37:31.000000 huhangkai-1.4.7/
--rw-rw-rw-   0        0        0      158 2023-07-03 16:37:31.000000 huhangkai-1.4.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 16:37:31.000000 huhangkai-1.4.7/commen/
--rw-rw-rw-   0        0        0      933 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:37:31.000000 huhangkai-1.4.7/commen/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/case_project/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/case_project/base_project.py
--rw-rw-rw-   0        0        0      803 2023-07-03 16:30:27.000000 huhangkai-1.4.7/commen/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-03 16:37:30.000000 huhangkai-1.4.7/commen/case_project/version.py
--rw-rw-rw-   0        0        0    29301 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/init_project.py
--rw-rw-rw-   0        0        0      244 2023-07-03 16:37:29.000000 huhangkai-1.4.7/commen/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:37:31.000000 huhangkai-1.4.7/commen/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:37:31.000000 huhangkai-1.4.7/commen/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3252 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     1348 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0     1548 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2148 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      568 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2609 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1696 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0      519 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      553 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    13338 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    23691 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-03 15:22:10.000000 huhangkai-1.4.7/commen/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-03 16:12:55.000000 huhangkai-1.4.7/commen/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:37:31.000000 huhangkai-1.4.7/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      158 2023-07-03 16:37:31.000000 huhangkai-1.4.7/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      972 2023-07-03 16:37:31.000000 huhangkai-1.4.7/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 16:37:31.000000 huhangkai-1.4.7/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-07-03 16:37:31.000000 huhangkai-1.4.7/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-03 16:37:31.000000 huhangkai-1.4.7/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 16:37:31.000000 huhangkai-1.4.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/
+-rw-rw-rw-   0        0        0      158 2023-07-03 16:38:23.000000 huhangkai-1.4.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/
+-rw-rw-rw-   0        0        0      933 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/case_project/base_project.py
+-rw-rw-rw-   0        0        0      803 2023-07-03 16:30:27.000000 huhangkai-1.4.8/commen/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/case_project/version.py
+-rw-rw-rw-   0        0        0    29301 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/init_project.py
+-rw-rw-rw-   0        0        0      276 2023-07-03 16:38:21.000000 huhangkai-1.4.8/commen/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/commen/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3252 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     1348 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0     1548 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2148 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      568 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2609 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1696 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0      519 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      553 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    13338 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_encryption.py
+-rw-rw-rw-   0        0        0    23691 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     9218 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-03 15:22:10.000000 huhangkai-1.4.8/commen/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-03 16:12:55.000000 huhangkai-1.4.8/commen/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      158 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      972 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-03 16:38:23.000000 huhangkai-1.4.8/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 16:38:23.000000 huhangkai-1.4.8/setup.cfg
```

### Comparing `huhangkai-1.4.7/commen/__init__.py` & `huhangkai-1.4.8/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/case_project/base_project.py` & `huhangkai-1.4.8/commen/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/case_project/setup_set.py` & `huhangkai-1.4.8/commen/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/init_project.py` & `huhangkai-1.4.8/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/data.py` & `huhangkai-1.4.8/commen/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/par_do.py` & `huhangkai-1.4.8/commen/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/test_cogroupbykey.py` & `huhangkai-1.4.8/commen/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/test_fiter.py` & `huhangkai-1.4.8/commen/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/test_flatmap.py` & `huhangkai-1.4.8/commen/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/test_map.py` & `huhangkai-1.4.8/commen/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/test_par_do.py` & `huhangkai-1.4.8/commen/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/test_regex.py` & `huhangkai-1.4.8/commen/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/test_time.py` & `huhangkai-1.4.8/commen/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/testcase/apache/test_to_string.py` & `huhangkai-1.4.8/commen/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/unit_apache_beam.py` & `huhangkai-1.4.8/commen/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/unit_dict.py` & `huhangkai-1.4.8/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/unit_encryption.py` & `huhangkai-1.4.8/commen/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/unit_fun.py` & `huhangkai-1.4.8/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/unit_logger.py` & `huhangkai-1.4.8/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/unit_request.py` & `huhangkai-1.4.8/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/unit_tasks.py` & `huhangkai-1.4.8/commen/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/commen/常用命令.py` & `huhangkai-1.4.8/commen/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.4.7/huhangkai.egg-info/SOURCES.txt` & `huhangkai-1.4.8/huhangkai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

