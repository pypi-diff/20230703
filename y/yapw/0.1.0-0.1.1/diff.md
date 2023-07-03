# Comparing `tmp/yapw-0.1.0.tar.gz` & `tmp/yapw-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapw-0.1.0.tar", last modified: Mon Jul  3 02:41:56 2023, max compression
+gzip compressed data, was "yapw-0.1.1.tar", last modified: Mon Jul  3 03:13:10 2023, max compression
```

## Comparing `yapw-0.1.0.tar` & `yapw-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-03 02:41:43.000000 yapw-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 02:41:43.000000 yapw-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-03 02:41:56.454431 yapw-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 02:41:43.000000 yapw-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.450431 yapw-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.450431 yapw-0.1.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/decorators.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/methods.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/types.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.450431 yapw-0.1.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-03 02:41:43.000000 yapw-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-03 02:41:56.454431 yapw-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_async_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_blocking_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/fixtures/busy.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/fixtures/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/fixtures/raiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/fixtures/sleeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/yapw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30057 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/ossignal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/yapw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:10.146586 yapw-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-03 03:13:01.000000 yapw-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 03:13:01.000000 yapw-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-03 03:13:10.146586 yapw-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 03:13:01.000000 yapw-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:10.142586 yapw-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:10.142586 yapw-0.1.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/api/clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/api/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/api/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/api/types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:10.142586 yapw-0.1.1/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 03:13:01.000000 yapw-0.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-03 03:13:01.000000 yapw-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-03 03:13:10.146586 yapw-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:10.142586 yapw-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:10.142586 yapw-0.1.1/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/clients/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/clients/test_async_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/clients/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/clients/test_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/clients/test_blocking_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:10.142586 yapw-0.1.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/fixtures/busy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/fixtures/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/fixtures/raiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/fixtures/sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 03:13:01.000000 yapw-0.1.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:10.146586 yapw-0.1.1/yapw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:01.000000 yapw-0.1.1/yapw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29989 2023-07-03 03:13:01.000000 yapw-0.1.1/yapw/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-03 03:13:01.000000 yapw-0.1.1/yapw/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-03 03:13:01.000000 yapw-0.1.1/yapw/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 03:13:01.000000 yapw-0.1.1/yapw/ossignal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:01.000000 yapw-0.1.1/yapw/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 03:13:01.000000 yapw-0.1.1/yapw/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 03:13:01.000000 yapw-0.1.1/yapw/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 03:13:10.146586 yapw-0.1.1/yapw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-03 03:13:10.000000 yapw-0.1.1/yapw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 03:13:10.000000 yapw-0.1.1/yapw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 03:13:10.000000 yapw-0.1.1/yapw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 03:13:10.000000 yapw-0.1.1/yapw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 03:13:10.000000 yapw-0.1.1/yapw.egg-info/top_level.txt
```

### Comparing `yapw-0.1.0/LICENSE` & `yapw-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/PKG-INFO` & `yapw-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapw
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Pika wrapper with error handling, signal handling and good defaults.
 Home-page: https://github.com/open-contracting/yapw
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `yapw-0.1.0/README.rst` & `yapw-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/docs/Makefile` & `yapw-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/docs/changelog.rst` & `yapw-0.1.1/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Changelog
 =========
 
-0.1.0 (2023-06-29)
+0.1.1 (2023-07-02)
+------------------
+
+Fixed
+~~~~~
+
+-  Fix logging of exchange type.
+
+0.1.0 (2023-07-02)
 ------------------
 
 Added
 ~~~~~
 
 -  :class:`yapw.clients.Async`
 -  :class:`yapw.clients.AsyncConsumer`
 -  :meth:`yapw.clients.Base.add_signal_handler`
 -  :meth:`yapw.clients.Base.interrupt`
 -  :meth:`yapw.clients.Base.state`
--  :meth:`yapw.clients.Blocking.channel_cancel`
+-  :meth:`yapw.clients.Blocking.channel_cancel_callback`
 -  :meth:`yapw.clients.Blocking.add_signal_handler`
 -  :meth:`yapw.clients.Blocking.interrupt`
 
 Changed
 ~~~~~~~
 
 **BREAKING CHANGES:**
```

### Comparing `yapw-0.1.0/docs/conf.py` & `yapw-0.1.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "Yet Another Pika Wrapper"
 copyright = "2021, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.1.0"
+version = "0.1.1"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `yapw-0.1.0/docs/index.rst` & `yapw-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/setup.cfg` & `yapw-0.1.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [flake8]
 max-line-length = 119
 extend-ignore = E203
 
 [metadata]
 name = yapw
-version = 0.1.0
+version = 0.1.1
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = A Pika wrapper with error handling, signal handling and good defaults.
 url = https://github.com/open-contracting/yapw
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `yapw-0.1.0/tests/__init__.py` & `yapw-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/clients/test_async.py` & `yapw-0.1.1/tests/clients/test_async.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/clients/test_async_consumer.py` & `yapw-0.1.1/tests/clients/test_async_consumer.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/clients/test_base.py` & `yapw-0.1.1/tests/clients/test_base.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/clients/test_blocking.py` & `yapw-0.1.1/tests/clients/test_blocking.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/clients/test_blocking_consumer.py` & `yapw-0.1.1/tests/clients/test_blocking_consumer.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/conftest.py` & `yapw-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/fixtures/busy.py` & `yapw-0.1.1/tests/fixtures/busy.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/fixtures/publisher.py` & `yapw-0.1.1/tests/fixtures/publisher.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/fixtures/raiser.py` & `yapw-0.1.1/tests/fixtures/raiser.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/fixtures/sleeper.py` & `yapw-0.1.1/tests/fixtures/sleeper.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/test_decorators.py` & `yapw-0.1.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/tests/test_methods.py` & `yapw-0.1.1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/yapw/clients.py` & `yapw-0.1.1/yapw/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,15 +519,15 @@
 
     def channel_qosok_callback(self, method: pika.frame.Method[pika.spec.Basic.QosOk]) -> None:
         """Declare the exchange, once the prefetch count is set."""
         if self.exchange:
             logger.debug(
                 "Declaring %s %s exchange %s",
                 "durable" if self.durable else "transient",
-                ExchangeType[self.exchange_type].value,  # type: ignore # "Enum index should be a string"
+                self.exchange_type,
                 self.exchange,
             )
             self.channel.exchange_declare(
                 exchange=self.exchange,
                 exchange_type=self.exchange_type,
                 durable=self.durable,
                 callback=self.exchange_declareok_callback,
@@ -625,15 +625,15 @@
         self.channel.queue_bind(queue=queue_name, exchange=self.exchange, routing_key=routing_key, callback=cb)
 
     def consume(self, on_message_callback: ConsumerCallback, decorator: Decorator, queue_name: str) -> None:
         """
         Start consuming messages from the queue.
 
         Run the consumer callback in separate threads, to not block the IO loop. (This assumes the consumer callback is
-        :py:ref:`CPU-bound<running-blocking-code>`.) Add signal handlers to wait for threads to terminate.
+        :py:ref:`CPU-bound<asyncio-handle-blocking>`.) Add signal handlers to wait for threads to terminate.
 
         The consumer callback is a function that accepts ``(state, channel, method, properties, body)`` arguments. The
         ``state`` argument contains thread-safe attributes. The rest of the arguments are the same as
         :meth:`pika.channel.Channel.basic_consume`'s ``on_message_callback``.
         """
         self.channel.add_on_cancel_callback(self.channel_cancel_callback)
```

### Comparing `yapw-0.1.0/yapw/decorators.py` & `yapw-0.1.1/yapw/decorators.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/yapw/methods.py` & `yapw-0.1.1/yapw/methods.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/yapw/types.py` & `yapw-0.1.1/yapw/types.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/yapw/util.py` & `yapw-0.1.1/yapw/util.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.0/yapw.egg-info/PKG-INFO` & `yapw-0.1.1/yapw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapw
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Pika wrapper with error handling, signal handling and good defaults.
 Home-page: https://github.com/open-contracting/yapw
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `yapw-0.1.0/yapw.egg-info/SOURCES.txt` & `yapw-0.1.1/yapw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

