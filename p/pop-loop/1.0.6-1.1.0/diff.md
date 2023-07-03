# Comparing `tmp/pop-loop-1.0.6.tar.gz` & `tmp/pop-loop-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-loop-1.0.6.tar", last modified: Thu Nov  3 23:03:03 2022, max compression
+gzip compressed data, was "pop-loop-1.1.0.tar", last modified: Mon Jul  3 20:19:01 2023, max compression
```

## Comparing `pop-loop-1.0.6.tar` & `pop-loop-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 23:03:03.068163 pop-loop-1.0.6/
--rw-r--r--   0 root         (0) root         (0)    11342 2022-11-03 23:02:41.000000 pop-loop-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4776 2022-11-03 23:03:03.068163 pop-loop-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3471 2022-11-03 23:02:41.000000 pop-loop-1.0.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 23:03:03.066163 pop-loop-1.0.6/pop_loop/
--rw-r--r--   0 root         (0) root         (0)      203 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 23:03:03.068163 pop-loop-1.0.6/pop_loop/loop/
--rw-r--r--   0 root         (0) root         (0)     1273 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/auto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 23:03:03.068163 pop-loop-1.0.6/pop_loop/loop/contracts/
--rw-r--r--   0 root         (0) root         (0)      434 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     1272 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/curio_loop.py
--rw-r--r--   0 root         (0) root         (0)     2176 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/init.py
--rw-r--r--   0 root         (0) root         (0)      727 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/proactor.py
--rw-r--r--   0 root         (0) root         (0)      526 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/qt.py
--rw-r--r--   0 root         (0) root         (0)      359 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/selector_unix.py
--rw-r--r--   0 root         (0) root         (0)      483 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/selector_win.py
--rw-r--r--   0 root         (0) root         (0)      414 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/tornado_loop.py
--rw-r--r--   0 root         (0) root         (0)      367 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/trio_loop.py
--rw-r--r--   0 root         (0) root         (0)      515 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/twisted_loop.py
--rw-r--r--   0 root         (0) root         (0)      304 2022-11-03 23:02:41.000000 pop-loop-1.0.6/pop_loop/loop/uv_loop.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-11-03 23:03:02.000000 pop-loop-1.0.6/pop_loop/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 23:03:03.067163 pop-loop-1.0.6/pop_loop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4776 2022-11-03 23:03:03.000000 pop-loop-1.0.6/pop_loop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      546 2022-11-03 23:03:03.000000 pop-loop-1.0.6/pop_loop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-03 23:03:03.000000 pop-loop-1.0.6/pop_loop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      466 2022-11-03 23:03:03.000000 pop-loop-1.0.6/pop_loop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-03 23:03:03.000000 pop-loop-1.0.6/pop_loop.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-03 23:03:03.069163 pop-loop-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3045 2022-11-03 23:02:41.000000 pop-loop-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:19:01.702289 pop-loop-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-07-03 20:18:46.000000 pop-loop-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4777 2023-07-03 20:19:01.702289 pop-loop-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-07-03 20:18:46.000000 pop-loop-1.1.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:19:01.702289 pop-loop-1.1.0/pop_loop/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:19:01.702289 pop-loop-1.1.0/pop_loop/loop/
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/auto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:19:01.702289 pop-loop-1.1.0/pop_loop/loop/contracts/
+-rw-r--r--   0 root         (0) root         (0)      434 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/curio_loop.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/init.py
+-rw-r--r--   0 root         (0) root         (0)      727 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/proactor.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/qt.py
+-rw-r--r--   0 root         (0) root         (0)      359 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/selector_unix.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/selector_win.py
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/tornado_loop.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/trio_loop.py
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/twisted_loop.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-03 20:18:46.000000 pop-loop-1.1.0/pop_loop/loop/uv_loop.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 20:19:01.000000 pop-loop-1.1.0/pop_loop/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 20:19:01.702289 pop-loop-1.1.0/pop_loop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4777 2023-07-03 20:19:01.000000 pop-loop-1.1.0/pop_loop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      546 2023-07-03 20:19:01.000000 pop-loop-1.1.0/pop_loop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 20:19:01.000000 pop-loop-1.1.0/pop_loop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      274 2023-07-03 20:19:01.000000 pop-loop-1.1.0/pop_loop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 20:19:01.000000 pop-loop-1.1.0/pop_loop.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 20:19:01.706289 pop-loop-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-07-03 20:18:46.000000 pop-loop-1.1.0/setup.py
```

### Comparing `pop-loop-1.0.6/LICENSE` & `pop-loop-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-loop-1.0.6/PKG-INFO` & `pop-loop-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: pop-loop
-Version: 1.0.6
+Version: 1.1.0
 Summary: Plugins that allow alternate io loops to be used to run asynchronous code in pop projects
 Home-page: https://vmware.gitlab.io/pop/pop-loop/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/pop-loop
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-loop/issues
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
-Provides-Extra: uvloop
+Provides-Extra: trio
 Provides-Extra: qt
-Provides-Extra: tornado
 Provides-Extra: curio
+Provides-Extra: uvloop
 Provides-Extra: twisted
-Provides-Extra: trio
+Provides-Extra: tornado
 License-File: LICENSE
 
 ========
 pop-loop
 ========
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
@@ -71,15 +71,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `pop-loop-1.0.6/README.rst` & `pop-loop-1.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `pop-loop-1.0.6/pop_loop/loop/auto.py` & `pop-loop-1.1.0/pop_loop/loop/auto.py`

 * *Files identical despite different names*

### Comparing `pop-loop-1.0.6/pop_loop/loop/curio_loop.py` & `pop-loop-1.1.0/pop_loop/loop/curio_loop.py`

 * *Files identical despite different names*

### Comparing `pop-loop-1.0.6/pop_loop/loop/init.py` & `pop-loop-1.1.0/pop_loop/loop/init.py`

 * *Files identical despite different names*

### Comparing `pop-loop-1.0.6/pop_loop/loop/proactor.py` & `pop-loop-1.1.0/pop_loop/loop/proactor.py`

 * *Files identical despite different names*

### Comparing `pop-loop-1.0.6/pop_loop/loop/qt.py` & `pop-loop-1.1.0/pop_loop/loop/qt.py`

 * *Files identical despite different names*

### Comparing `pop-loop-1.0.6/pop_loop/loop/twisted_loop.py` & `pop-loop-1.1.0/pop_loop/loop/twisted_loop.py`

 * *Files identical despite different names*

### Comparing `pop-loop-1.0.6/pop_loop.egg-info/PKG-INFO` & `pop-loop-1.1.0/pop_loop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: pop-loop
-Version: 1.0.6
+Version: 1.1.0
 Summary: Plugins that allow alternate io loops to be used to run asynchronous code in pop projects
 Home-page: https://vmware.gitlab.io/pop/pop-loop/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/pop-loop
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/pop-loop/issues
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
-Provides-Extra: uvloop
+Provides-Extra: trio
 Provides-Extra: qt
-Provides-Extra: tornado
 Provides-Extra: curio
+Provides-Extra: uvloop
 Provides-Extra: twisted
-Provides-Extra: trio
+Provides-Extra: tornado
 License-File: LICENSE
 
 ========
 pop-loop
 ========
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
@@ -71,15 +71,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `pop-loop-1.0.6/pop_loop.egg-info/SOURCES.txt` & `pop-loop-1.1.0/pop_loop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop-loop-1.0.6/setup.py` & `pop-loop-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,26 +72,26 @@
     },
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     license="Apache Software License 2.0",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
     ],
     packages=discover_packages(),
     cmdclass={"clean": Clean},
 )
```

