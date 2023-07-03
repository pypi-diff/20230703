# Comparing `tmp/yapw-0.1.2.tar.gz` & `tmp/yapw-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapw-0.1.2.tar", last modified: Mon Jul  3 04:52:13 2023, max compression
+gzip compressed data, was "yapw-0.1.3.tar", last modified: Mon Jul  3 19:06:18 2023, max compression
```

## Comparing `yapw-0.1.2.tar` & `yapw-0.1.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:13.583026 yapw-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-03 04:52:02.000000 yapw-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 04:52:02.000000 yapw-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-03 04:52:13.583026 yapw-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 04:52:02.000000 yapw-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:13.575026 yapw-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:13.575026 yapw-0.1.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/api/clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/api/decorators.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/api/methods.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/api/types.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:13.575026 yapw-0.1.2/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 04:52:02.000000 yapw-0.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-03 04:52:02.000000 yapw-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 04:52:13.583026 yapw-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:13.579026 yapw-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:13.579026 yapw-0.1.2/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/clients/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/clients/test_async_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/clients/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/clients/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/clients/test_blocking_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:13.579026 yapw-0.1.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/fixtures/busy.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/fixtures/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/fixtures/raiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/fixtures/sleeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 04:52:02.000000 yapw-0.1.2/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:13.579026 yapw-0.1.2/yapw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:02.000000 yapw-0.1.2/yapw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29989 2023-07-03 04:52:02.000000 yapw-0.1.2/yapw/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-03 04:52:02.000000 yapw-0.1.2/yapw/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-03 04:52:02.000000 yapw-0.1.2/yapw/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 04:52:02.000000 yapw-0.1.2/yapw/ossignal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:02.000000 yapw-0.1.2/yapw/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-03 04:52:02.000000 yapw-0.1.2/yapw/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 04:52:02.000000 yapw-0.1.2/yapw/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:52:13.583026 yapw-0.1.2/yapw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-03 04:52:13.000000 yapw-0.1.2/yapw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 04:52:13.000000 yapw-0.1.2/yapw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:52:13.000000 yapw-0.1.2/yapw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 04:52:13.000000 yapw-0.1.2/yapw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 04:52:13.000000 yapw-0.1.2/yapw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:18.124181 yapw-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-03 19:06:09.000000 yapw-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 19:06:09.000000 yapw-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-03 19:06:18.124181 yapw-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 19:06:09.000000 yapw-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:18.120181 yapw-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:18.120181 yapw-0.1.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/api/clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/api/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/api/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/api/types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:18.120181 yapw-0.1.3/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:06:09.000000 yapw-0.1.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-03 19:06:09.000000 yapw-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 19:06:18.128181 yapw-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:18.124181 yapw-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:18.124181 yapw-0.1.3/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/clients/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/clients/test_async_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/clients/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/clients/test_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/clients/test_blocking_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:18.124181 yapw-0.1.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/fixtures/busy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/fixtures/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/fixtures/raiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/fixtures/sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 19:06:09.000000 yapw-0.1.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:18.124181 yapw-0.1.3/yapw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:09.000000 yapw-0.1.3/yapw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30473 2023-07-03 19:06:09.000000 yapw-0.1.3/yapw/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-03 19:06:09.000000 yapw-0.1.3/yapw/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-03 19:06:09.000000 yapw-0.1.3/yapw/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 19:06:09.000000 yapw-0.1.3/yapw/ossignal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:09.000000 yapw-0.1.3/yapw/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-03 19:06:09.000000 yapw-0.1.3/yapw/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 19:06:09.000000 yapw-0.1.3/yapw/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:18.124181 yapw-0.1.3/yapw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-03 19:06:18.000000 yapw-0.1.3/yapw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 19:06:18.000000 yapw-0.1.3/yapw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:06:18.000000 yapw-0.1.3/yapw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 19:06:18.000000 yapw-0.1.3/yapw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 19:06:18.000000 yapw-0.1.3/yapw.egg-info/top_level.txt
```

### Comparing `yapw-0.1.2/LICENSE` & `yapw-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/PKG-INFO` & `yapw-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapw
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Pika wrapper with error handling, signal handling and good defaults.
 Home-page: https://github.com/open-contracting/yapw
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `yapw-0.1.2/README.rst` & `yapw-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/docs/Makefile` & `yapw-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/docs/changelog.rst` & `yapw-0.1.3/docs/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+0.1.3 (2023-07-03)
+------------------
+
+Changed
+~~~~~~~
+
+-  :meth:`yapw.clients.Async.connection_open_error_callback`: Don't retry if the error is an authentication (e.g. incorrect username or password) or access denied (e.g. non-existent virtual host) error.
+-  :meth:`yapw.clients.Async.connection_close_callback`: Change log level from ``ERROR`` to ``WARNING``.
+-  :meth:`yapw.clients.Async` log messages format errors with ``%r`` instead of ``%s``, to include information like the exception class.
+
 0.1.2 (2023-07-02)
 ------------------
 
 Added
 ~~~~~
 
 -  Restore Python 3.10 support.
```

### Comparing `yapw-0.1.2/docs/conf.py` & `yapw-0.1.3/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "Yet Another Pika Wrapper"
 copyright = "2021, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.1.2"
+version = "0.1.3"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `yapw-0.1.2/docs/index.rst` & `yapw-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/setup.cfg` & `yapw-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [flake8]
 max-line-length = 119
 extend-ignore = E203
 
 [metadata]
 name = yapw
-version = 0.1.2
+version = 0.1.3
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = A Pika wrapper with error handling, signal handling and good defaults.
 url = https://github.com/open-contracting/yapw
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `yapw-0.1.2/tests/__init__.py` & `yapw-0.1.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/clients/test_async_consumer.py` & `yapw-0.1.3/tests/clients/test_async_consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,29 +74,29 @@
     assert consumer.connection.is_closed
 
     assert len(caplog.records) == 4
     assert [(r.levelname, r.message) for r in caplog.records] == [
         ("INFO", "Sleep"),
         ("INFO", f"Received {signame}, shutting down gracefully"),
         ("INFO", "Wake!"),
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')"),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'"),
     ]
 
 
 def test_decode_valid(short_message, short_timer, caplog):
     consumer = async_consumer(on_message_callback=ack_warner, queue="q", decode=functools.partial(decode, 0))
     consumer.start()
 
     assert consumer.channel.is_closed
     assert consumer.connection.is_closed
 
     assert len(caplog.records) == 2
     assert [(r.levelname, r.message) for r in caplog.records] == [
         ("WARNING", "1"),
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')"),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'"),
     ]
 
 
 def test_decode_invalid(short_message, timer, caplog):
     caplog.set_level(logging.INFO)
 
     consumer = async_consumer(
@@ -106,15 +106,15 @@
 
     assert consumer.channel.is_closed
     assert consumer.connection.is_closed
 
     assert len(caplog.records) == 2
     assert [(r.levelname, r.message, r.exc_info is None) for r in caplog.records] == [
         ("ERROR", f"{encode(short_message)} can't be decoded, shutting down gracefully", False),
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')", True),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'", True),
     ]
 
 
 def test_decode_raiser(message, timer, caplog):
     caplog.set_level(logging.INFO)
 
     consumer = async_consumer(on_message_callback=ack_warner, queue="q", decode=raiser)
@@ -122,15 +122,15 @@
 
     assert consumer.channel.is_closed
     assert consumer.connection.is_closed
 
     assert len(caplog.records) == 2
     assert [(r.levelname, r.message, r.exc_info is None) for r in caplog.records] == [
         ("ERROR", f"{encode(message)} can't be decoded, shutting down gracefully", False),
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')", True),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'", True),
     ]
 
 
 def test_halt(message, timer, caplog):
     caplog.set_level(logging.INFO)
 
     consumer = async_consumer(on_message_callback=raiser, queue="q")
@@ -138,15 +138,15 @@
 
     assert consumer.channel.is_closed
     assert consumer.connection.is_closed
 
     assert len(caplog.records) == 2
     assert [(r.levelname, r.message, r.exc_info is None) for r in caplog.records] == [
         ("ERROR", f"Unhandled exception when consuming {encode(message)}, shutting down gracefully", False),
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')", True),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'", True),
     ]
 
 
 def test_discard(message, short_timer, caplog):
     caplog.set_level(logging.INFO)
 
     consumer = async_consumer(on_message_callback=raiser, queue="q", decorator=discard)
@@ -155,15 +155,15 @@
     assert consumer.channel.is_closed
     assert consumer.connection.is_closed
 
     assert len(caplog.records) == 3
     assert [(r.levelname, r.message, r.exc_info is None) for r in caplog.records] == [
         ("ERROR", f"Unhandled exception when consuming {encode(message)}, discarding message", False),
         ("INFO", "Received SIGINT, shutting down gracefully", True),
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')", True),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'", True),
     ]
 
 
 def test_requeue(message, short_timer, caplog):
     caplog.set_level(logging.INFO)
 
     consumer = async_consumer(on_message_callback=raiser, queue="q", decorator=requeue)
@@ -173,15 +173,15 @@
     assert consumer.connection.is_closed
 
     assert len(caplog.records) == 4
     assert [(r.levelname, r.message, r.exc_info is None) for r in caplog.records] == [
         ("ERROR", f"Unhandled exception when consuming {encode(message)} (requeue=True)", False),
         ("ERROR", f"Unhandled exception when consuming {encode(message)} (requeue=False)", False),
         ("INFO", "Received SIGINT, shutting down gracefully", True),
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')", True),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'", True),
     ]
 
 
 def test_publish(message, short_timer, caplog):
     caplog.set_level(logging.DEBUG)
 
     consumer = async_consumer(on_message_callback=writer, queue="q", exchange_type="direct")
@@ -197,15 +197,15 @@
         ("DEBUG", f"Received message {encode(message)} with routing key yapw_test_q and delivery tag 1"),
         (
             "DEBUG",
             "Published message {'message': 'value'} on channel 1 to exchange yapw_test with routing key yapw_test_n",
         ),
         ("DEBUG", "Ack'd message on channel 1 with delivery tag 1"),
         ("INFO", "Received SIGINT, shutting down gracefully"),
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')"),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'"),
     ]
 
 
 def test_consume_declares_queue(caplog):
     with timed(DELAY):
         declarer = async_consumer(on_message_callback=raiser, queue="q")
         declarer.start()
@@ -226,15 +226,15 @@
     assert consumer.connection.is_closed
 
     assert len(caplog.records[start:end]) > 1
     assert all(r.levelname == "WARNING" and r.message == "{'message': 'value'}" for r in caplog.records[start:end])
 
     for i, j in ((0, start), (end, len(caplog.records))):
         assert [(r.levelname, r.message) for r in caplog.records[i:j]] == [
-            ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')"),
+            ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'"),
         ]
 
 
 def test_consume_declares_queue_routing_keys(caplog):
     with timed(DELAY):
         declarer = async_consumer(on_message_callback="raiser", queue="q", routing_keys=["r", "k"])
         declarer.start()
@@ -251,12 +251,12 @@
     publisher.close()
 
     assert consumer.channel.is_closed
     assert consumer.connection.is_closed
 
     assert len(caplog.records) == 4
     assert [(r.levelname, r.message) for r in caplog.records] == [
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')"),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'"),
         ("WARNING", "{'message': 'r'}"),
         ("WARNING", "{'message': 'k'}"),
-        ("WARNING", "Channel 1 was closed: (0, 'Normal shutdown')"),
+        ("WARNING", "Channel 1 was closed: ChannelClosedByClient: (0) 'Normal shutdown'"),
     ]
```

### Comparing `yapw-0.1.2/tests/clients/test_base.py` & `yapw-0.1.3/tests/clients/test_base.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/clients/test_blocking.py` & `yapw-0.1.3/tests/clients/test_blocking.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/clients/test_blocking_consumer.py` & `yapw-0.1.3/tests/clients/test_blocking_consumer.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/conftest.py` & `yapw-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/fixtures/busy.py` & `yapw-0.1.3/tests/fixtures/busy.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/fixtures/publisher.py` & `yapw-0.1.3/tests/fixtures/publisher.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/fixtures/raiser.py` & `yapw-0.1.3/tests/fixtures/raiser.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/fixtures/sleeper.py` & `yapw-0.1.3/tests/fixtures/sleeper.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/test_decorators.py` & `yapw-0.1.3/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/tests/test_methods.py` & `yapw-0.1.3/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/yapw/clients.py` & `yapw-0.1.3/yapw/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from collections import namedtuple
 from collections.abc import Callable
 from concurrent.futures import ThreadPoolExecutor
 from types import FrameType
 from typing import Any, Generic, TypeVar
 
 import pika
-import pika.exceptions
 from pika.adapters.asyncio_connection import AsyncioConnection
+from pika.exceptions import ProbableAccessDeniedError, ProbableAuthenticationError
 from pika.exchange_type import ExchangeType
 
 from yapw.decorators import halt
 from yapw.ossignal import signal_names
 from yapw.types import ConsumerCallback, Decode, Decorator, Encode, State
 from yapw.util import basic_publish_debug_args, basic_publish_kwargs, default_decode, default_encode
 
@@ -441,23 +441,30 @@
         """
         self.executor = ThreadPoolExecutor(thread_name_prefix=f"yapw-{self.thread_name_infix}")
         self.blocked = False
         self.consumer_tag = ""
 
     def connection_open_error_callback(self, connection: pika.connection.Connection, error: Exception | str) -> None:
         """Retry, once the connection couldn't be established."""
-        logger.error("Connection failed, retrying in %ds: %s", self.RECONNECT_DELAY, error)
-        self.connection.ioloop.call_later(self.RECONNECT_DELAY, self.reconnect)
+        if isinstance(error, (ProbableAccessDeniedError, ProbableAuthenticationError)):
+            logger.error("Stopping: %r", error)
+            self.connection.ioloop.stop()
+        else:
+            logger.error("Connection failed, retrying in %ds: %r", self.RECONNECT_DELAY, error)
+            self.connection.ioloop.call_later(self.RECONNECT_DELAY, self.reconnect)
 
     def connection_close_callback(self, connection: pika.connection.Connection, reason: Exception) -> None:
         """Reconnect, if the connection was closed unexpectedly. Otherwise, stop the IO loop."""
         if self.stopping:
+            # A message has been logged, prior to calling interrupt().
             self.connection.ioloop.stop()
         else:
-            logger.error("Connection closed, reconnecting in %ds: %s", self.RECONNECT_DELAY, reason)
+            # For example: ConnectionClosedByBroker: (320) "CONNECTION_FORCED - broker forced connection closure with
+            # reason 'shutdown'"
+            logger.warning("Connection closed, reconnecting in %ds: %r", self.RECONNECT_DELAY, reason)
             self.connection.ioloop.call_later(self.RECONNECT_DELAY, self.reconnect)
 
     def add_signal_handler(self, signalnum: int, handler: Callable[..., object]) -> None:
         """
         Add a handler for a signal.
         """
         self.connection.ioloop.add_signal_handler(signalnum, functools.partial(handler, signalnum=signalnum))
@@ -506,15 +513,15 @@
     def channel_close_callback(self, channel: pika.channel.Channel, reason: Exception) -> None:
         """
         Close the connection, once the client cancelled the consumer or once RabbitMQ closed the channel due to, e.g.,
         redeclaring exchanges with inconsistent parameters.
 
         A warning is logged, in case it was the latter.
         """
-        logger.warning("Channel %i was closed: %s", channel, reason)
+        logger.warning("Channel %i was closed: %r", channel, reason)
         # pika's connection.close() closes all channels. It can update the connection state before this callback runs.
         if not self.connection.is_closed and not self.connection.is_closing:
             # The channel is already closed. Free any resources, without waiting for threads.
             self.executor.shutdown(wait=False, cancel_futures=True)
             self.connection.close()
 
     def channel_qosok_callback(self, method: pika.frame.Method[pika.spec.Basic.QosOk]) -> None:
```

### Comparing `yapw-0.1.2/yapw/decorators.py` & `yapw-0.1.3/yapw/decorators.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/yapw/methods.py` & `yapw-0.1.3/yapw/methods.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/yapw/types.py` & `yapw-0.1.3/yapw/types.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/yapw/util.py` & `yapw-0.1.3/yapw/util.py`

 * *Files identical despite different names*

### Comparing `yapw-0.1.2/yapw.egg-info/PKG-INFO` & `yapw-0.1.3/yapw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yapw
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Pika wrapper with error handling, signal handling and good defaults.
 Home-page: https://github.com/open-contracting/yapw
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `yapw-0.1.2/yapw.egg-info/SOURCES.txt` & `yapw-0.1.3/yapw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

