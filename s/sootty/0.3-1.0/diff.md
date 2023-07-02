# Comparing `tmp/sootty-0.3.tar.gz` & `tmp/sootty-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sootty-0.3.tar", last modified: Mon Apr 17 01:13:50 2023, max compression
+gzip compressed data, was "dist/sootty-1.0.tar", last modified: Sun Jul  2 22:37:03 2023, max compression
```

## Comparing `sootty-0.3.tar` & `sootty-1.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2021-10-21 07:58:08.000000 sootty-0.3/MANIFEST.in
--rw-r--r--   0 benjamin   (501) staff       (20)     5785 2023-04-17 01:13:50.000000 sootty-0.3/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)     4480 2023-04-17 00:26:55.000000 sootty-0.3/README.md
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-04-17 01:13:50.000000 sootty-0.3/setup.cfg
--rw-r--r--   0 benjamin   (501) staff       (20)      865 2023-04-17 01:12:47.000000 sootty-0.3/setup.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/sootty/
--rw-r--r--   0 benjamin   (501) staff       (20)      206 2022-01-17 06:44:06.000000 sootty-0.3/sootty/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     5045 2022-11-11 21:06:02.000000 sootty-0.3/sootty/__main__.py
--rw-r--r--   0 benjamin   (501) staff       (20)      789 2022-01-17 06:54:19.000000 sootty-0.3/sootty/display.py
--rw-r--r--   0 benjamin   (501) staff       (20)      197 2022-01-17 06:54:19.000000 sootty-0.3/sootty/exceptions.py
--rw-r--r--   0 benjamin   (501) staff       (20)     2566 2022-09-20 06:13:12.000000 sootty-0.3/sootty/parser.py
--rw-r--r--   0 benjamin   (501) staff       (20)     2192 2022-09-20 06:13:12.000000 sootty-0.3/sootty/save.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/sootty/static/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2021-10-01 21:29:54.000000 sootty-0.3/sootty/static/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     1103 2022-11-11 21:06:02.000000 sootty-0.3/sootty/static/grammar.lark
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/sootty/storage/
--rw-r--r--   0 benjamin   (501) staff       (20)      126 2022-01-17 06:48:58.000000 sootty-0.3/sootty/storage/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     6243 2022-11-11 20:12:51.000000 sootty-0.3/sootty/storage/valuechange.py
--rw-r--r--   0 benjamin   (501) staff       (20)     5693 2022-11-11 20:12:51.000000 sootty-0.3/sootty/storage/wire.py
--rw-r--r--   0 benjamin   (501) staff       (20)     1771 2022-11-11 21:06:02.000000 sootty-0.3/sootty/storage/wiregroup.py
--rw-r--r--   0 benjamin   (501) staff       (20)    13157 2022-11-11 21:06:02.000000 sootty-0.3/sootty/storage/wiretrace.py
--rw-r--r--   0 benjamin   (501) staff       (20)    15024 2022-09-20 06:13:12.000000 sootty-0.3/sootty/utils.py
--rw-r--r--   0 benjamin   (501) staff       (20)    40240 2022-11-11 21:33:17.000000 sootty-0.3/sootty/visualizer.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/sootty.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)     5785 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      679 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       49 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/entry_points.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       41 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       12 2023-04-17 01:13:49.000000 sootty-0.3/sootty.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-17 01:13:50.000000 sootty-0.3/test/
--rw-r--r--   0 benjamin   (501) staff       (20)      216 2022-11-11 21:40:39.000000 sootty-0.3/test/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)      215 2022-11-11 21:21:24.000000 sootty-0.3/test/test_all.py
--rw-r--r--   0 benjamin   (501) staff       (20)     1241 2022-11-11 21:40:49.000000 sootty-0.3/test/test_general.py
--rw-r--r--   0 benjamin   (501) staff       (20)      988 2022-11-11 21:28:20.000000 sootty-0.3/test/test_limits.py
--rw-r--r--   0 benjamin   (501) staff       (20)     2840 2022-11-11 21:35:18.000000 sootty-0.3/test/test_pyrtl.py
--rw-r--r--   0 benjamin   (501) staff       (20)      647 2022-11-11 21:37:11.000000 sootty-0.3/test/test_style.py
--rw-r--r--   0 benjamin   (501) staff       (20)      303 2022-11-11 21:32:01.000000 sootty-0.3/test/test_wires.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-02 22:37:03.000000 sootty-1.0/
+-rw-r--r--   0 benjamin   (501) staff       (20)     1524 2021-10-21 07:58:08.000000 sootty-1.0/LICENSE
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2021-10-21 07:58:08.000000 sootty-1.0/MANIFEST.in
+-rw-r--r--   0 benjamin   (501) staff       (20)     5785 2023-07-02 22:37:03.000000 sootty-1.0/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)     4480 2023-04-17 01:16:54.000000 sootty-1.0/README.md
+-rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-07-02 22:37:03.000000 sootty-1.0/setup.cfg
+-rw-r--r--   0 benjamin   (501) staff       (20)      888 2023-07-02 22:36:56.000000 sootty-1.0/setup.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-02 22:37:03.000000 sootty-1.0/sootty/
+-rw-r--r--   0 benjamin   (501) staff       (20)      206 2022-01-17 06:44:06.000000 sootty-1.0/sootty/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     5045 2022-11-11 21:06:02.000000 sootty-1.0/sootty/__main__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      789 2022-01-17 06:54:19.000000 sootty-1.0/sootty/display.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      197 2022-01-17 06:54:19.000000 sootty-1.0/sootty/exceptions.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     2566 2022-09-20 06:13:12.000000 sootty-1.0/sootty/parser.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     2192 2022-09-20 06:13:12.000000 sootty-1.0/sootty/save.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-02 22:37:03.000000 sootty-1.0/sootty/static/
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2021-10-01 21:29:54.000000 sootty-1.0/sootty/static/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1103 2022-11-11 21:06:02.000000 sootty-1.0/sootty/static/grammar.lark
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-02 22:37:03.000000 sootty-1.0/sootty/storage/
+-rw-r--r--   0 benjamin   (501) staff       (20)      126 2022-01-17 06:48:58.000000 sootty-1.0/sootty/storage/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     6243 2022-11-11 20:12:51.000000 sootty-1.0/sootty/storage/valuechange.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     5693 2022-11-11 20:12:51.000000 sootty-1.0/sootty/storage/wire.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1771 2022-11-11 21:06:02.000000 sootty-1.0/sootty/storage/wiregroup.py
+-rw-r--r--   0 benjamin   (501) staff       (20)    13157 2023-07-02 20:41:17.000000 sootty-1.0/sootty/storage/wiretrace.py
+-rw-r--r--   0 benjamin   (501) staff       (20)    15024 2022-09-20 06:13:12.000000 sootty-1.0/sootty/utils.py
+-rw-r--r--   0 benjamin   (501) staff       (20)    40240 2023-04-17 01:16:54.000000 sootty-1.0/sootty/visualizer.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-02 22:37:03.000000 sootty-1.0/sootty.egg-info/
+-rw-r--r--   0 benjamin   (501) staff       (20)     5785 2023-07-02 22:37:03.000000 sootty-1.0/sootty.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)      687 2023-07-02 22:37:03.000000 sootty-1.0/sootty.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-07-02 22:37:03.000000 sootty-1.0/sootty.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       49 2023-07-02 22:37:03.000000 sootty-1.0/sootty.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       53 2023-07-02 22:37:03.000000 sootty-1.0/sootty.egg-info/requires.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)       12 2023-07-02 22:37:03.000000 sootty-1.0/sootty.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-02 22:37:03.000000 sootty-1.0/test/
+-rw-r--r--   0 benjamin   (501) staff       (20)      216 2023-04-17 01:16:54.000000 sootty-1.0/test/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      215 2023-04-17 01:16:54.000000 sootty-1.0/test/test_all.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1241 2023-04-17 01:16:54.000000 sootty-1.0/test/test_general.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      988 2023-04-17 01:16:54.000000 sootty-1.0/test/test_limits.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     2840 2023-04-17 01:16:54.000000 sootty-1.0/test/test_pyrtl.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      647 2023-04-17 01:16:54.000000 sootty-1.0/test/test_style.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      303 2023-04-17 01:16:54.000000 sootty-1.0/test/test_wires.py
```

### Comparing `sootty-0.3/PKG-INFO` & `sootty-1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sootty
-Version: 0.3
+Version: 1.0
 Summary: Displays vcd files to the command line.
 Home-page: https://github.com/Ben1152000/sootty
 Author: Ben Darnell
 Author-email: ben@bdarnell.com
 License: BSD
 Description: # Sootty
```

### Comparing `sootty-0.3/README.md` & `sootty-1.0/README.md`

 * *Files identical despite different names*

### Comparing `sootty-0.3/setup.py` & `sootty-1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text(encoding='utf-8')
 
 
 setuptools.setup( 
     name='sootty',
-    version='0.3',
+    version='1.0',
     description='Displays vcd files to the command line.', 
     long_description=README,
     packages=setuptools.find_packages(exclude=("tests",)), 
     long_description_content_type="text/markdown",
     url="https://github.com/Ben1152000/sootty",
     author="Ben Darnell",
     author_email="ben@bdarnell.com",
@@ -26,10 +26,11 @@
     },
     package_data={
         "sootty.static": ["*.lark"],
     },
     install_requires=[
         'lark>=1',
         'pyvcd>=0.3',
-        'sortedcontainers>=2.4'
+        'sortedcontainers>=2.4',
+        'PyYAML>=6.0'
     ],
 )
```

### Comparing `sootty-0.3/sootty/__main__.py` & `sootty-1.0/sootty/__main__.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/display.py` & `sootty-1.0/sootty/display.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/parser.py` & `sootty-1.0/sootty/parser.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/save.py` & `sootty-1.0/sootty/save.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/static/grammar.lark` & `sootty-1.0/sootty/static/grammar.lark`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/storage/valuechange.py` & `sootty-1.0/sootty/storage/valuechange.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/storage/wire.py` & `sootty-1.0/sootty/storage/wire.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/storage/wiregroup.py` & `sootty-1.0/sootty/storage/wiregroup.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/storage/wiretrace.py` & `sootty-1.0/sootty/storage/wiretrace.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/utils.py` & `sootty-1.0/sootty/utils.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty/visualizer.py` & `sootty-1.0/sootty/visualizer.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/sootty.egg-info/PKG-INFO` & `sootty-1.0/sootty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sootty
-Version: 0.3
+Version: 1.0
 Summary: Displays vcd files to the command line.
 Home-page: https://github.com/Ben1152000/sootty
 Author: Ben Darnell
 Author-email: ben@bdarnell.com
 License: BSD
 Description: # Sootty
```

### Comparing `sootty-0.3/sootty.egg-info/SOURCES.txt` & `sootty-1.0/sootty.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 sootty/__init__.py
 sootty/__main__.py
 sootty/display.py
 sootty/exceptions.py
```

### Comparing `sootty-0.3/test/test_general.py` & `sootty-1.0/test/test_general.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/test/test_limits.py` & `sootty-1.0/test/test_limits.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/test/test_pyrtl.py` & `sootty-1.0/test/test_pyrtl.py`

 * *Files identical despite different names*

### Comparing `sootty-0.3/test/test_style.py` & `sootty-1.0/test/test_style.py`

 * *Files identical despite different names*

