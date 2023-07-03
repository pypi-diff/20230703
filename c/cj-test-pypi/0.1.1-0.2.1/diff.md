# Comparing `tmp/cj_test_pypi-0.1.1.tar.gz` & `tmp/cj_test_pypi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cj_test_pypi-0.1.1.tar", last modified: Mon Jul  3 11:38:03 2023, max compression
+gzip compressed data, was "dist/cj_test_pypi-0.2.1.tar", last modified: Mon Jul  3 11:50:03 2023, max compression
```

## Comparing `cj_test_pypi-0.1.1.tar` & `cj_test_pypi-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-03 11:38:03.708977 cj_test_pypi-0.1.1/
--rw-r--r--   0 bytedance   (502) staff       (20)      567 2023-07-03 11:38:03.708714 cj_test_pypi-0.1.1/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)        5 2023-07-03 07:59:09.000000 cj_test_pypi-0.1.1/README.md
-drwxr-xr-x   0 bytedance   (502) staff       (20)        0 2023-07-03 11:38:03.708266 cj_test_pypi-0.1.1/cj_test_pypi.egg-info/
--rw-r--r--   0 bytedance   (502) staff       (20)      567 2023-07-03 11:38:03.000000 cj_test_pypi-0.1.1/cj_test_pypi.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (502) staff       (20)      197 2023-07-03 11:38:03.000000 cj_test_pypi-0.1.1/cj_test_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-07-03 11:38:03.000000 cj_test_pypi-0.1.1/cj_test_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       70 2023-07-03 11:38:03.000000 cj_test_pypi-0.1.1/cj_test_pypi.egg-info/requires.txt
--rw-r--r--   0 bytedance   (502) staff       (20)        1 2023-07-03 11:38:03.000000 cj_test_pypi-0.1.1/cj_test_pypi.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (502) staff       (20)       38 2023-07-03 11:38:03.709058 cj_test_pypi-0.1.1/setup.cfg
--rw-r--r--   0 bytedance   (502) staff       (20)     1721 2023-07-03 08:15:56.000000 cj_test_pypi-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/cj_test_pypi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      531 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/cj_test_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/cj_test_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/cj_test_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/cj_test_pypi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/cj_test_pypi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-07-03 11:50:03.000000 cj_test_pypi-0.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `cj_test_pypi-0.1.1/PKG-INFO` & `cj_test_pypi-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: cj_test_pypi
-Version: 0.1.1
+Version: 0.2.1
 Summary: cj_test_pypi
 Home-page: https://www.cj_test_pypi.com/
 Author: chenjing
 Author-email: 471476942@qq.com
-License: UNKNOWN
 Keywords: boilerplate
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 
 #test
-
```

### Comparing `cj_test_pypi-0.1.1/cj_test_pypi.egg-info/PKG-INFO` & `cj_test_pypi-0.2.1/cj_test_pypi.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: cj-test-pypi
-Version: 0.1.1
+Version: 0.2.1
 Summary: cj_test_pypi
 Home-page: https://www.cj_test_pypi.com/
 Author: chenjing
 Author-email: 471476942@qq.com
-License: UNKNOWN
 Keywords: boilerplate
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 
 #test
-
```

### Comparing `cj_test_pypi-0.1.1/setup.py` & `cj_test_pypi-0.2.1/setup.py`

 * *Files identical despite different names*

