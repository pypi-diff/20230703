# Comparing `tmp/hello_world_cc2-0.0.8.tar.gz` & `tmp/hello_world_cc2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_world_cc2-0.0.8.tar", last modified: Mon Jul  3 15:43:53 2023, max compression
+gzip compressed data, was "hello_world_cc2-0.0.9.tar", last modified: Mon Jul  3 15:47:32 2023, max compression
```

## Comparing `hello_world_cc2-0.0.8.tar` & `hello_world_cc2-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 15:43:53.807546 hello_world_cc2-0.0.8/
--rw-r--r--   0 chenchen   (501) staff       (20)     3078 2023-06-28 07:04:50.000000 hello_world_cc2-0.0.8/.gitignore
--rw-r--r--   0 chenchen   (501) staff       (20)    11357 2023-06-28 07:04:50.000000 hello_world_cc2-0.0.8/LICENSE
--rw-r--r--   0 chenchen   (501) staff       (20)    13889 2023-07-03 15:43:53.807340 hello_world_cc2-0.0.8/PKG-INFO
--rw-r--r--   0 chenchen   (501) staff       (20)      679 2023-07-03 10:57:13.000000 hello_world_cc2-0.0.8/README.md
-drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 15:43:53.806171 hello_world_cc2-0.0.8/hello_world/
--rw-r--r--   0 chenchen   (501) staff       (20)       97 2023-07-03 15:43:25.000000 hello_world_cc2-0.0.8/hello_world/__init__.py
--rw-r--r--   0 chenchen   (501) staff       (20)     3852 2023-07-03 15:03:22.000000 hello_world_cc2-0.0.8/hello_world/client.py
-drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 15:43:53.807029 hello_world_cc2-0.0.8/hello_world_cc2.egg-info/
--rw-r--r--   0 chenchen   (501) staff       (20)    13889 2023-07-03 15:43:53.000000 hello_world_cc2-0.0.8/hello_world_cc2.egg-info/PKG-INFO
--rw-r--r--   0 chenchen   (501) staff       (20)      283 2023-07-03 15:43:53.000000 hello_world_cc2-0.0.8/hello_world_cc2.egg-info/SOURCES.txt
--rw-r--r--   0 chenchen   (501) staff       (20)        1 2023-07-03 15:43:53.000000 hello_world_cc2-0.0.8/hello_world_cc2.egg-info/dependency_links.txt
--rw-r--r--   0 chenchen   (501) staff       (20)       19 2023-07-03 15:43:53.000000 hello_world_cc2-0.0.8/hello_world_cc2.egg-info/requires.txt
--rw-r--r--   0 chenchen   (501) staff       (20)       12 2023-07-03 15:43:53.000000 hello_world_cc2-0.0.8/hello_world_cc2.egg-info/top_level.txt
--rw-r--r--   0 chenchen   (501) staff       (20)      432 2023-07-03 15:43:41.000000 hello_world_cc2-0.0.8/pyproject.toml
--rw-r--r--   0 chenchen   (501) staff       (20)       38 2023-07-03 15:43:53.807597 hello_world_cc2-0.0.8/setup.cfg
+drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 15:47:32.971403 hello_world_cc2-0.0.9/
+-rw-r--r--   0 chenchen   (501) staff       (20)     3078 2023-06-28 07:04:50.000000 hello_world_cc2-0.0.9/.gitignore
+-rw-r--r--   0 chenchen   (501) staff       (20)    11357 2023-06-28 07:04:50.000000 hello_world_cc2-0.0.9/LICENSE
+-rw-r--r--   0 chenchen   (501) staff       (20)    13889 2023-07-03 15:47:32.971178 hello_world_cc2-0.0.9/PKG-INFO
+-rw-r--r--   0 chenchen   (501) staff       (20)      679 2023-07-03 10:57:13.000000 hello_world_cc2-0.0.9/README.md
+drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 15:47:32.969692 hello_world_cc2-0.0.9/hello_world/
+-rw-r--r--   0 chenchen   (501) staff       (20)       93 2023-07-03 15:47:14.000000 hello_world_cc2-0.0.9/hello_world/__init__.py
+-rw-r--r--   0 chenchen   (501) staff       (20)     3852 2023-07-03 15:03:22.000000 hello_world_cc2-0.0.9/hello_world/client.py
+drwxr-xr-x   0 chenchen   (501) staff       (20)        0 2023-07-03 15:47:32.970892 hello_world_cc2-0.0.9/hello_world_cc2.egg-info/
+-rw-r--r--   0 chenchen   (501) staff       (20)    13889 2023-07-03 15:47:32.000000 hello_world_cc2-0.0.9/hello_world_cc2.egg-info/PKG-INFO
+-rw-r--r--   0 chenchen   (501) staff       (20)      283 2023-07-03 15:47:32.000000 hello_world_cc2-0.0.9/hello_world_cc2.egg-info/SOURCES.txt
+-rw-r--r--   0 chenchen   (501) staff       (20)        1 2023-07-03 15:47:32.000000 hello_world_cc2-0.0.9/hello_world_cc2.egg-info/dependency_links.txt
+-rw-r--r--   0 chenchen   (501) staff       (20)       19 2023-07-03 15:47:32.000000 hello_world_cc2-0.0.9/hello_world_cc2.egg-info/requires.txt
+-rw-r--r--   0 chenchen   (501) staff       (20)       12 2023-07-03 15:47:32.000000 hello_world_cc2-0.0.9/hello_world_cc2.egg-info/top_level.txt
+-rw-r--r--   0 chenchen   (501) staff       (20)      432 2023-07-03 15:47:22.000000 hello_world_cc2-0.0.9/pyproject.toml
+-rw-r--r--   0 chenchen   (501) staff       (20)       38 2023-07-03 15:47:32.971454 hello_world_cc2-0.0.9/setup.cfg
```

### Comparing `hello_world_cc2-0.0.8/.gitignore` & `hello_world_cc2-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hello_world_cc2-0.0.8/LICENSE` & `hello_world_cc2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hello_world_cc2-0.0.8/PKG-INFO` & `hello_world_cc2-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello_world_cc2
-Version: 0.0.8
+Version: 0.0.9
 Summary: the Official W3bstream Client for Python
 Author: haaai
 Author-email: chenchen <chen1233216@hotmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `hello_world_cc2-0.0.8/README.md` & `hello_world_cc2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hello_world_cc2-0.0.8/hello_world/client.py` & `hello_world_cc2-0.0.9/hello_world/client.py`

 * *Files identical despite different names*

### Comparing `hello_world_cc2-0.0.8/hello_world_cc2.egg-info/PKG-INFO` & `hello_world_cc2-0.0.9/hello_world_cc2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello-world-cc2
-Version: 0.0.8
+Version: 0.0.9
 Summary: the Official W3bstream Client for Python
 Author: haaai
 Author-email: chenchen <chen1233216@hotmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

