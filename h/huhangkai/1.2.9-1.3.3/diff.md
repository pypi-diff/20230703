# Comparing `tmp/huhangkai-1.2.9.tar.gz` & `tmp/huhangkai-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.2.9.tar", last modified: Mon Jul  3 11:48:21 2023, max compression
+gzip compressed data, was "huhangkai-1.3.3.tar", last modified: Mon Jul  3 11:57:26 2023, max compression
```

## Comparing `huhangkai-1.2.9.tar` & `huhangkai-1.3.3.tar`

### file list

```diff
@@ -1,40 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 11:48:21.276087 huhangkai-1.2.9/
--rw-rw-rw-   0        0        0      228 2023-07-03 11:48:21.276087 huhangkai-1.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 11:48:21.238672 huhangkai-1.2.9/commen/
--rw-rw-rw-   0        0        0      933 2023-06-20 02:22:12.000000 huhangkai-1.2.9/commen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 11:48:21.245653 huhangkai-1.2.9/commen/case_project/
--rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.2.9/commen/case_project/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-06-20 09:33:09.000000 huhangkai-1.2.9/commen/case_project/base_project.py
--rw-rw-rw-   0        0        0       17 2023-07-03 11:48:20.000000 huhangkai-1.2.9/commen/case_project/version.py
--rw-rw-rw-   0        0        0    29301 2023-06-20 08:10:42.000000 huhangkai-1.2.9/commen/init_project.py
--rw-rw-rw-   0        0        0      733 2023-07-03 11:46:34.000000 huhangkai-1.2.9/commen/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 11:48:21.246651 huhangkai-1.2.9/commen/testcase/
--rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.2.9/commen/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 11:48:21.266113 huhangkai-1.2.9/commen/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.2.9/commen/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3252 2023-07-03 09:00:44.000000 huhangkai-1.2.9/commen/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-01 21:14:54.000000 huhangkai-1.2.9/commen/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     1348 2023-07-03 08:59:15.000000 huhangkai-1.2.9/commen/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0     1548 2023-07-03 08:59:15.000000 huhangkai-1.2.9/commen/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2148 2023-07-03 08:59:24.000000 huhangkai-1.2.9/commen/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      568 2023-07-03 08:59:32.000000 huhangkai-1.2.9/commen/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2609 2023-07-03 09:13:27.000000 huhangkai-1.2.9/commen/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1696 2023-07-03 09:00:16.000000 huhangkai-1.2.9/commen/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0      519 2023-07-03 09:00:24.000000 huhangkai-1.2.9/commen/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      553 2023-07-03 09:00:34.000000 huhangkai-1.2.9/commen/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    13338 2023-07-03 09:47:06.000000 huhangkai-1.2.9/commen/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-05-25 08:37:49.000000 huhangkai-1.2.9/commen/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-05-25 08:46:34.000000 huhangkai-1.2.9/commen/unit_encryption.py
--rw-rw-rw-   0        0        0    23691 2023-07-03 11:39:14.000000 huhangkai-1.2.9/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-25 08:37:49.000000 huhangkai-1.2.9/commen/unit_logger.py
--rw-rw-rw-   0        0        0     9218 2023-06-02 10:02:56.000000 huhangkai-1.2.9/commen/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-06-29 01:27:06.000000 huhangkai-1.2.9/commen/unit_tasks.py
--rw-rw-rw-   0        0        0      725 2023-07-03 11:03:49.000000 huhangkai-1.2.9/commen/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-03 11:48:21.274092 huhangkai-1.2.9/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-07-03 11:48:21.000000 huhangkai-1.2.9/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      944 2023-07-03 11:48:21.000000 huhangkai-1.2.9/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 11:48:21.000000 huhangkai-1.2.9/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-03 11:48:21.000000 huhangkai-1.2.9/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-03 11:48:21.000000 huhangkai-1.2.9/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 11:48:21.277085 huhangkai-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0      144 2023-07-03 11:46:34.000000 huhangkai-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:57:26.554972 huhangkai-1.3.3/
+-rw-rw-rw-   0        0        0      228 2023-07-03 11:57:26.553948 huhangkai-1.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 11:57:26.522033 huhangkai-1.3.3/case_project/
+-rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.3.3/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-06-20 09:33:09.000000 huhangkai-1.3.3/case_project/base_project.py
+-rw-rw-rw-   0        0        0       17 2023-07-03 11:57:26.000000 huhangkai-1.3.3/case_project/version.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:57:26.530012 huhangkai-1.3.3/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-03 11:57:26.000000 huhangkai-1.3.3/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-07-03 11:57:26.000000 huhangkai-1.3.3/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 11:57:26.000000 huhangkai-1.3.3/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-03 11:57:26.000000 huhangkai-1.3.3/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-03 11:57:26.000000 huhangkai-1.3.3/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 11:57:26.554972 huhangkai-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-07-03 11:46:34.000000 huhangkai-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:57:26.532007 huhangkai-1.3.3/testcase/
+-rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.3.3/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 11:57:26.551954 huhangkai-1.3.3/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-06-20 03:37:01.000000 huhangkai-1.3.3/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3252 2023-07-03 09:00:44.000000 huhangkai-1.3.3/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-01 21:14:54.000000 huhangkai-1.3.3/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     1348 2023-07-03 08:59:15.000000 huhangkai-1.3.3/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0     1548 2023-07-03 08:59:15.000000 huhangkai-1.3.3/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2148 2023-07-03 08:59:24.000000 huhangkai-1.3.3/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      568 2023-07-03 08:59:32.000000 huhangkai-1.3.3/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2609 2023-07-03 09:13:27.000000 huhangkai-1.3.3/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1696 2023-07-03 09:00:16.000000 huhangkai-1.3.3/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0      519 2023-07-03 09:00:24.000000 huhangkai-1.3.3/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      553 2023-07-03 09:00:34.000000 huhangkai-1.3.3/testcase/apache/test_to_string.py
```

### Comparing `huhangkai-1.2.9/commen/case_project/base_project.py` & `huhangkai-1.3.3/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/setup.py` & `huhangkai-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/data.py` & `huhangkai-1.3.3/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/par_do.py` & `huhangkai-1.3.3/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/test_cogroupbykey.py` & `huhangkai-1.3.3/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/test_fiter.py` & `huhangkai-1.3.3/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/test_flatmap.py` & `huhangkai-1.3.3/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/test_map.py` & `huhangkai-1.3.3/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/test_par_do.py` & `huhangkai-1.3.3/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/test_regex.py` & `huhangkai-1.3.3/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/test_time.py` & `huhangkai-1.3.3/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.2.9/commen/testcase/apache/test_to_string.py` & `huhangkai-1.3.3/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

