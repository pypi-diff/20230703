# Comparing `tmp/pyRserve-1.0.1.tar.gz` & `tmp/pyRserve-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRserve-1.0.1.tar", last modified: Wed Jan 11 17:35:12 2023, max compression
+gzip compressed data, was "pyRserve-1.0.2.tar", last modified: Mon Jul  3 09:38:49 2023, max compression
```

## Comparing `pyRserve-1.0.1.tar` & `pyRserve-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 heinkel   (1000) users      (100)        0 2023-01-11 17:35:12.968479 pyRserve-1.0.1/
--rw-r--r--   0 heinkel   (1000) users      (100)     1169 2021-06-22 19:15:15.000000 pyRserve-1.0.1/LICENSE
--rw-r--r--   0 heinkel   (1000) users      (100)     5496 2023-01-11 17:35:12.968479 pyRserve-1.0.1/PKG-INFO
--rw-r--r--   0 heinkel   (1000) users      (100)     4092 2022-10-13 12:46:20.000000 pyRserve-1.0.1/README.rst
-drwxr-xr-x   0 heinkel   (1000) users      (100)        0 2023-01-11 17:35:12.968479 pyRserve-1.0.1/pyRserve/
--rw-r--r--   0 heinkel   (1000) users      (100)      563 2022-12-03 20:04:49.000000 pyRserve-1.0.1/pyRserve/__init__.py
--rw-r--r--   0 heinkel   (1000) users      (100)     2288 2022-12-03 20:04:49.000000 pyRserve-1.0.1/pyRserve/misc.py
--rw-r--r--   0 heinkel   (1000) users      (100)    16449 2022-12-03 20:04:49.000000 pyRserve-1.0.1/pyRserve/rconn.py
--rw-r--r--   0 heinkel   (1000) users      (100)      485 2022-12-03 20:04:49.000000 pyRserve-1.0.1/pyRserve/rexceptions.py
--rw-r--r--   0 heinkel   (1000) users      (100)    25642 2023-01-11 17:33:49.000000 pyRserve-1.0.1/pyRserve/rparser.py
--rw-r--r--   0 heinkel   (1000) users      (100)    17306 2022-12-03 20:04:49.000000 pyRserve-1.0.1/pyRserve/rserializer.py
--rw-r--r--   0 heinkel   (1000) users      (100)    14652 2022-12-03 20:04:49.000000 pyRserve-1.0.1/pyRserve/rtypes.py
--rw-r--r--   0 heinkel   (1000) users      (100)    11791 2022-12-03 20:04:49.000000 pyRserve-1.0.1/pyRserve/taggedContainers.py
--rw-r--r--   0 heinkel   (1000) users      (100)        6 2023-01-11 17:33:49.000000 pyRserve-1.0.1/pyRserve/version.txt
-drwxr-xr-x   0 heinkel   (1000) users      (100)        0 2023-01-11 17:35:12.968479 pyRserve-1.0.1/pyRserve.egg-info/
--rw-r--r--   0 heinkel   (1000) users      (100)     5496 2023-01-11 17:35:12.000000 pyRserve-1.0.1/pyRserve.egg-info/PKG-INFO
--rw-r--r--   0 heinkel   (1000) users      (100)      389 2023-01-11 17:35:12.000000 pyRserve-1.0.1/pyRserve.egg-info/SOURCES.txt
--rw-r--r--   0 heinkel   (1000) users      (100)        1 2023-01-11 17:35:12.000000 pyRserve-1.0.1/pyRserve.egg-info/dependency_links.txt
--rw-r--r--   0 heinkel   (1000) users      (100)       70 2023-01-11 17:35:12.000000 pyRserve-1.0.1/pyRserve.egg-info/requires.txt
--rw-r--r--   0 heinkel   (1000) users      (100)        9 2023-01-11 17:35:12.000000 pyRserve-1.0.1/pyRserve.egg-info/top_level.txt
--rw-r--r--   0 heinkel   (1000) users      (100)      187 2023-01-11 17:35:12.968479 pyRserve-1.0.1/setup.cfg
--rw-r--r--   0 heinkel   (1000) users      (100)     2108 2022-10-13 16:20:43.000000 pyRserve-1.0.1/setup.py
+drwxr-xr-x   0 heinkel   (1000) heinkel   (1000)        0 2023-07-03 09:38:49.582800 pyRserve-1.0.2/
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     1169 2023-03-28 19:22:37.000000 pyRserve-1.0.2/LICENSE
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     5492 2023-07-03 09:38:49.582800 pyRserve-1.0.2/PKG-INFO
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     4088 2023-07-01 11:52:38.000000 pyRserve-1.0.2/README.rst
+drwxr-xr-x   0 heinkel   (1000) heinkel   (1000)        0 2023-07-03 09:38:49.582800 pyRserve-1.0.2/pyRserve/
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)      563 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/__init__.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     2288 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/misc.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    16449 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rconn.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)      485 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rexceptions.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    25642 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rparser.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    17306 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rserializer.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    14652 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/rtypes.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)    11791 2023-03-28 19:22:37.000000 pyRserve-1.0.2/pyRserve/taggedContainers.py
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)        6 2023-07-01 14:31:55.000000 pyRserve-1.0.2/pyRserve/version.txt
+drwxr-xr-x   0 heinkel   (1000) heinkel   (1000)        0 2023-07-03 09:38:49.582800 pyRserve-1.0.2/pyRserve.egg-info/
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     5492 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/PKG-INFO
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)      389 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/SOURCES.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)        1 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/dependency_links.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)       70 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/requires.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)        9 2023-07-03 09:38:49.000000 pyRserve-1.0.2/pyRserve.egg-info/top_level.txt
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)      187 2023-07-03 09:38:49.582800 pyRserve-1.0.2/setup.cfg
+-rw-r--r--   0 heinkel   (1000) heinkel   (1000)     2108 2023-07-01 14:29:24.000000 pyRserve-1.0.2/setup.py
```

### Comparing `pyRserve-1.0.1/LICENSE` & `pyRserve-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.1/PKG-INFO` & `pyRserve-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRserve
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python client to remotely access the R statistic package via network
 Home-page: https://github.com/ralhei/pyRserve
 Author: Ralph Heinkel
 Author-email: rh@ralph-heinkel.com
 License: MIT license
 Project-URL: Documentation, https://pyrserve.readthedocs.io/
 Project-URL: Changelog, https://pyrserve.readthedocs.io/en/latest/changelog.html
@@ -41,15 +41,15 @@
 
 pyRserve is a library for connecting Python to `R  <http://www.r-project.org/>`_
 (an excellent statistic package). Running `Rserve <http://www.rforge.net/Rserve/>`_
 in R attaches the R-interpreter to a network socket, waiting for pyRserve to connect to it.
 Through such a connection, variables can be get and set in R from Python,
 and also R-functions can be called remotely.
 
-In contrast to `rpy or rpy2 <http://rpy.sourceforge.net/>`_ the R process does not have to
+In contrast to `rpy or rpy2 <https://rpy2.github.io/>`_ the R process does not have to
 run on the same machine, it can run on a remote machine and all variable  access and
 function calls will be delegated there through the network.
 
 Furthermore - and this makes everything feel very pythonic - all data structures will
 automatically be converted from native R to native Python and numpy types and back.
```

### Comparing `pyRserve-1.0.1/README.rst` & `pyRserve-1.0.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 pyRserve is a library for connecting Python to `R  <http://www.r-project.org/>`_
 (an excellent statistic package). Running `Rserve <http://www.rforge.net/Rserve/>`_
 in R attaches the R-interpreter to a network socket, waiting for pyRserve to connect to it.
 Through such a connection, variables can be get and set in R from Python,
 and also R-functions can be called remotely.
 
-In contrast to `rpy or rpy2 <http://rpy.sourceforge.net/>`_ the R process does not have to
+In contrast to `rpy or rpy2 <https://rpy2.github.io/>`_ the R process does not have to
 run on the same machine, it can run on a remote machine and all variable  access and
 function calls will be delegated there through the network.
 
 Furthermore - and this makes everything feel very pythonic - all data structures will
 automatically be converted from native R to native Python and numpy types and back.
```

### Comparing `pyRserve-1.0.1/pyRserve/__init__.py` & `pyRserve-1.0.2/pyRserve/__init__.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.1/pyRserve/misc.py` & `pyRserve-1.0.2/pyRserve/misc.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.1/pyRserve/rconn.py` & `pyRserve-1.0.2/pyRserve/rconn.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.1/pyRserve/rparser.py` & `pyRserve-1.0.2/pyRserve/rparser.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.1/pyRserve/rserializer.py` & `pyRserve-1.0.2/pyRserve/rserializer.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.1/pyRserve/rtypes.py` & `pyRserve-1.0.2/pyRserve/rtypes.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.1/pyRserve/taggedContainers.py` & `pyRserve-1.0.2/pyRserve/taggedContainers.py`

 * *Files identical despite different names*

### Comparing `pyRserve-1.0.1/pyRserve.egg-info/PKG-INFO` & `pyRserve-1.0.2/pyRserve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRserve
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python client to remotely access the R statistic package via network
 Home-page: https://github.com/ralhei/pyRserve
 Author: Ralph Heinkel
 Author-email: rh@ralph-heinkel.com
 License: MIT license
 Project-URL: Documentation, https://pyrserve.readthedocs.io/
 Project-URL: Changelog, https://pyrserve.readthedocs.io/en/latest/changelog.html
@@ -41,15 +41,15 @@
 
 pyRserve is a library for connecting Python to `R  <http://www.r-project.org/>`_
 (an excellent statistic package). Running `Rserve <http://www.rforge.net/Rserve/>`_
 in R attaches the R-interpreter to a network socket, waiting for pyRserve to connect to it.
 Through such a connection, variables can be get and set in R from Python,
 and also R-functions can be called remotely.
 
-In contrast to `rpy or rpy2 <http://rpy.sourceforge.net/>`_ the R process does not have to
+In contrast to `rpy or rpy2 <https://rpy2.github.io/>`_ the R process does not have to
 run on the same machine, it can run on a remote machine and all variable  access and
 function calls will be delegated there through the network.
 
 Furthermore - and this makes everything feel very pythonic - all data structures will
 automatically be converted from native R to native Python and numpy types and back.
```

### Comparing `pyRserve-1.0.1/setup.py` & `pyRserve-1.0.2/setup.py`

 * *Files identical despite different names*

