# Comparing `tmp/yapw-0.0.9.tar.gz` & `tmp/yapw-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapw-0.0.9.tar", last modified: Mon Jan 24 22:27:58 2022, max compression
+gzip compressed data, was "yapw-0.1.0.tar", last modified: Mon Jul  3 02:41:56 2023, max compression
```

## Comparing `yapw-0.0.9.tar` & `yapw-0.1.0.tar`

### file list

```diff
@@ -1,58 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.454838 yapw-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-01-24 22:27:52.000000 yapw-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-01-24 22:27:52.000000 yapw-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-01-24 22:27:58.454838 yapw-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-01-24 22:27:52.000000 yapw-0.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.450838 yapw-0.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.450838 yapw-0.0.9/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/api/clients.rst
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/api/decorators.rst
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/api/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.450838 yapw-0.0.9/docs/api/methods/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/api/methods/blocking.rst
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/api/methods/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/api/types.rst
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2681 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.450838 yapw-0.0.9/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6784 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-24 22:27:52.000000 yapw-0.0.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-01-24 22:27:52.000000 yapw-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-24 22:27:58.454838 yapw-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-01-24 22:27:52.000000 yapw-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.450838 yapw-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.450838 yapw-0.0.9/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/clients/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/clients/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (121)     3586 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/clients/test_publisher.py
--rw-r--r--   0 runner    (1001) docker     (121)     9078 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/clients/test_threaded.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.450838 yapw-0.0.9/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/fixtures/raiser.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/fixtures/sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.450838 yapw-0.0.9/tests/methods/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3771 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/methods/test_blocking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5985 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-01-24 22:27:52.000000 yapw-0.0.9/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.454838 yapw-0.0.9/yapw/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:52.000000 yapw-0.0.9/yapw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12391 2022-01-24 22:27:52.000000 yapw-0.0.9/yapw/clients.py
--rw-r--r--   0 runner    (1001) docker     (121)     5580 2022-01-24 22:27:52.000000 yapw-0.0.9/yapw/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.454838 yapw-0.0.9/yapw/methods/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:52.000000 yapw-0.0.9/yapw/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2840 2022-01-24 22:27:52.000000 yapw-0.0.9/yapw/methods/blocking.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-01-24 22:27:52.000000 yapw-0.0.9/yapw/ossignal.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:52.000000 yapw-0.0.9/yapw/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-01-24 22:27:52.000000 yapw-0.0.9/yapw/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2918 2022-01-24 22:27:52.000000 yapw-0.0.9/yapw/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-24 22:27:58.454838 yapw-0.0.9/yapw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-01-24 22:27:58.000000 yapw-0.0.9/yapw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-01-24 22:27:58.000000 yapw-0.0.9/yapw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-24 22:27:58.000000 yapw-0.0.9/yapw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-01-24 22:27:58.000000 yapw-0.0.9/yapw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-24 22:27:58.000000 yapw-0.0.9/yapw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-03 02:41:43.000000 yapw-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 02:41:43.000000 yapw-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-03 02:41:56.454431 yapw-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 02:41:43.000000 yapw-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.450431 yapw-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.450431 yapw-0.1.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.450431 yapw-0.1.0/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 02:41:43.000000 yapw-0.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-03 02:41:43.000000 yapw-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-03 02:41:56.454431 yapw-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_async_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/clients/test_blocking_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/fixtures/busy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/fixtures/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/fixtures/raiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/fixtures/sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 02:41:43.000000 yapw-0.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/yapw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30057 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/ossignal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-03 02:41:43.000000 yapw-0.1.0/yapw/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:41:56.454431 yapw-0.1.0/yapw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 02:41:56.000000 yapw-0.1.0/yapw.egg-info/top_level.txt
```

### Comparing `yapw-0.0.9/LICENSE` & `yapw-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yapw-0.0.9/PKG-INFO` & `yapw-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: yapw
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Pika wrapper with error handling, signal handling and good defaults.
 Home-page: https://github.com/open-contracting/yapw
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: perf
 Provides-Extra: test
 Provides-Extra: types
 Provides-Extra: docs
 License-File: LICENSE
 
 |PyPI Version| |Build Status| |Coverage Status| |Python Version|
 
-Yet Another Pika Wrapper (yapw – pronounced yapu) makes it easier to create a `Pika <https://pika.readthedocs.io/en/stable/>`__ client that has error handling, signal handling, useful logging and good defaults.
+Yet Another Pika Wrapper (yapw – pronounced yapu) makes it easier to create a `Pika <https://pika.readthedocs.io/en/stable/>`__ client that:
+
+-  Runs consumer callbacks in separate threads.
+-  Automatically decodes and encodes messages.
+-  Has error handling, signal handling, useful logging and good defaults.
 
 (If you are viewing this on GitHub, open the `full documentation <https://yapw.readthedocs.io/>`__ for additional details.)
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/yapw.svg
    :target: https://pypi.org/project/yapw/
 .. |Build Status| image:: https://github.com/open-contracting/yapw/workflows/CI/badge.svg
    :target: https://github.com/open-contracting/yapw/actions?query=workflow%3ACI
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/yapw/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/yapw?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/yapw.svg
    :target: https://pypi.org/project/yapw/
-
-
```

### Comparing `yapw-0.0.9/docs/Makefile` & `yapw-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yapw-0.0.9/docs/conf.py` & `yapw-0.1.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,29 @@
 # -- Project information -----------------------------------------------------
 
 project = "Yet Another Pika Wrapper"
 copyright = "2021, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.0.9"
+version = "0.1.0"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
+    "sphinx_design",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
```

### Comparing `yapw-0.0.9/tests/methods/test_blocking.py` & `yapw-0.1.0/tests/test_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 from collections import namedtuple
 from unittest.mock import create_autospec
 
 import pika
 import pytest
 
-from yapw.methods.blocking import ack, nack, publish
+from yapw.methods import ack, nack, publish
 from yapw.util import default_encode
 
 Connection = namedtuple("Connection", "is_open add_callback_threadsafe")
 Channel = namedtuple("Channel", "channel_number is_open basic_ack basic_nack basic_publish")
 State = namedtuple("State", "format_routing_key connection exchange encode content_type delivery_mode")
 
 ack_nack_parameters = [(ack, "ack", [1]), (nack, "nack", [1])]
```

### Comparing `yapw-0.0.9/tests/test_decorators.py` & `yapw-0.1.0/tests/test_decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
-import signal
 from collections import namedtuple
 from unittest.mock import Mock, patch
 
 import pytest
 
-from yapw.decorators import decorate, default_decode, discard, requeue
+from yapw.decorators import decorate, discard, requeue
+from yapw.util import default_decode
 
 # https://pika.readthedocs.io/en/stable/modules/spec.html#pika.spec.Basic.Deliver
 Deliver = namedtuple("Deliver", "delivery_tag redelivered routing_key")
 # https://pika.readthedocs.io/en/stable/modules/spec.html#pika.spec.BasicProperties
 BasicProperties = namedtuple("BasicProperties", "content_type")
 
 logger = logging.getLogger(__name__)
@@ -80,30 +80,27 @@
     assert caplog.records[-1].levelname == "DEBUG"
     assert caplog.records[-1].message == "Received message b'message value' with routing key key and delivery tag 1"
 
 
 def test_decode_invalid(caplog):
     caplog.set_level(logging.DEBUG)
 
-    function = Mock()
-    signal.signal(signal.SIGUSR2, function)
-
+    state = Mock()
     method = Deliver(1, False, "key")
     properties = BasicProperties("application/json")
 
-    discard(default_decode, passes, "state", "channel", method, properties, b"invalid")
+    discard(default_decode, passes, state, "channel", method, properties, b"invalid")
 
-    function.assert_called_once()
-    assert function.call_args[0][0] == signal.SIGUSR2
+    state.connection.ioloop.call_soon_threadsafe.assert_called_once_with(state.interrupt)
 
     assert len(caplog.records) == 2
     assert caplog.records[0].levelname == "DEBUG"
     assert caplog.records[0].message == "Received message b'invalid' with routing key key and delivery tag 1"
     assert caplog.records[-1].levelname == "ERROR"
-    assert caplog.records[-1].message == "b'invalid' can't be decoded, sending SIGUSR2"
+    assert caplog.records[-1].message == "b'invalid' can't be decoded, shutting down gracefully"
     assert caplog.records[-1].exc_info
 
 
 @patch("yapw.decorators.nack")
 def test_discard(nack, caplog):
     caplog.set_level(logging.DEBUG)
```

### Comparing `yapw-0.0.9/yapw/decorators.py` & `yapw-0.1.0/yapw/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,158 +1,142 @@
 """
 Decorators to be used with consumer callbacks.
 
 A message must be ack'd or nack'd if using `consumer prefetch <https://www.rabbitmq.com/consumer-prefetch.html>`__,
 because otherwise `RabbitMQ stops delivering messages <https://www.rabbitmq.com/confirms.html#channel-qos-prefetch>`__.
 The decorators help to ensure that, in case of error, either the message is nack'd or the process is halted.
 
-:func:`~yapw.decorators.halt` is the default decorator. For example, if a callback inserts messages into a database,
-and the database is down, but this exception isn't handled by the callback, then the :func:`~yapw.decorators.discard`
-or :func:`~yapw.decorators.requeue` decorators would end up nack'ing all messages in the queue. The ``halt`` decorator
-instead stops the consumer, so that an administrator can decide when it is appropriate to restart it.
+:func:`~yapw.decorators.halt` is the default decorator. It stops the consumer and halts the process, so that an
+administrator can decide when it is appropriate to restart it.
 
-Decorators look like this (see :func:`~yapw.decorators.decorate` for context):
+The other decorators require more care. For example, if a callback inserts messages into a database, and the database
+is down, but this exception isn't handled by the callback, then the :func:`~yapw.decorators.discard` or
+:func:`~yapw.decorators.requeue` decorators would end up nack'ing all messages in the queue.
+
+Decorators look like this (see the :func:`~yapw.decorators.decorate` function for context):
 
 .. code-block:: python
 
    from yapw.decorators import decorate
 
 
    def myfunction(decode, callback, state, channel, method, properties, body):
        def errback(exception):
            # do something, like halting the process or nack'ing the message
 
        decorate(decode, callback, state, channel, method, properties, body, errback)
-
-User-defined decorators should avoid doing work outside the ``finally`` branch. Do work in the callback.
 """
 from __future__ import annotations
 
 import logging
-import os
-import signal
-from typing import Any, Callable, Optional
+from collections.abc import Callable
+from typing import Any
 
 import pika
 
-from yapw.methods.blocking import nack
+from yapw.methods import add_callback_threadsafe, nack
 from yapw.types import ConsumerCallback, Decode, State
-from yapw.util import jsonlib
 
 logger = logging.getLogger(__name__)
 
 
-def default_decode(body: bytes, content_type: Optional[str]) -> Any:
-    """
-    If the content type is "application/json", deserializes the JSON formatted bytes to a Python object. Otherwise,
-    returns the bytes (which the consumer callback can deserialize independently).
-
-    Uses `orjson <https://pypi.org/project/orjson/>`__ if available.
-
-    :param body: the encoded message
-    :param content_type: the message's content type
-    :returns: a Python object
-    """
-    if content_type == "application/json":
-        return jsonlib.loads(body)
-    return body
-
-
 def decorate(
     decode: Decode,
     callback: ConsumerCallback,
-    state: State,
+    state: State[Any],
     channel: pika.channel.Channel,
     method: pika.spec.Basic.Deliver,
     properties: pika.BasicProperties,
     body: bytes,
     errback: Callable[[Exception], None],
-    finalback: Optional[Callable[[], None]] = None,
+    finalback: Callable[[], None] | None = None,
 ) -> None:
     """
+    Use this function to define your own decorators.
+
     Decode the message ``body`` using the ``decode`` function, and call the consumer ``callback``.
 
     If the ``callback`` function raises an exception, call the ``errback`` function. In any case, call the
     ``finalback`` function after calling the ``callback`` function.
 
-    If the ``decode`` function raises an exception, send the SIGUSR2 signal to the main thread.
+    If the ``decode`` function raises an exception, shut down the client in the main thread.
 
     .. seealso::
 
-       :meth:`yapw.clients.Threaded.consume` for details on the consumer callback function signature.
+       :mod:`yapw.clients` for details on the consumer callback function signature.
     """
     logger.debug(
         "Received message %s with routing key %s and delivery tag %s", body, method.routing_key, method.delivery_tag
     )
     try:
         message = decode(body, properties.content_type)
         try:
             callback(state, channel, method, properties, message)
         except Exception as exception:
             errback(exception)
         finally:
             if finalback:
                 finalback()
     except Exception:
-        logger.exception("%r can't be decoded, sending SIGUSR2", body)
-        os.kill(os.getpid(), signal.SIGUSR2)
+        logger.exception("%r can't be decoded, shutting down gracefully", body)
+        add_callback_threadsafe(state.connection, state.interrupt)
 
 
 # https://stackoverflow.com/a/7099229/244258
 def halt(
     decode: Decode,
     callback: ConsumerCallback,
-    state: State,
+    state: State[Any],
     channel: pika.channel.Channel,
     method: pika.spec.Basic.Deliver,
     properties: pika.BasicProperties,
     body: bytes,
 ) -> None:
     """
-    If the callback raises an exception, send the SIGUSR1 signal to the main thread, without acknowledgment.
+    If the ``callback`` function raises an exception, shut down the client in the main thread, without acknowledgment.
     """
 
     def errback(exception: Exception) -> None:
-        logger.exception("Unhandled exception when consuming %r, sending SIGUSR1", body)
-        os.kill(os.getpid(), signal.SIGUSR1)
+        logger.exception("Unhandled exception when consuming %r, shutting down gracefully", body)
+        add_callback_threadsafe(state.connection, state.interrupt)
 
     decorate(decode, callback, state, channel, method, properties, body, errback)
 
 
 def discard(
     decode: Decode,
     callback: ConsumerCallback,
-    state: State,
+    state: State[Any],
     channel: pika.channel.Channel,
     method: pika.spec.Basic.Deliver,
     properties: pika.BasicProperties,
     body: bytes,
 ) -> None:
     """
-    If the callback raises an exception, nack the message without requeueing.
+    If the ``callback`` function raises an exception, nack the message, without requeueing.
     """
 
     def errback(exception: Exception) -> None:
         logger.exception("Unhandled exception when consuming %r, discarding message", body)
         nack(state, channel, method.delivery_tag, requeue=False)
 
     decorate(decode, callback, state, channel, method, properties, body, errback)
 
 
 def requeue(
     decode: Decode,
     callback: ConsumerCallback,
-    state: State,
+    state: State[Any],
     channel: pika.channel.Channel,
     method: pika.spec.Basic.Deliver,
     properties: pika.BasicProperties,
     body: bytes,
 ) -> None:
     """
-    If the callback raises an exception, nack the message, and requeue the message unless it was redelivered.
+    If the ``callback`` function raises an exception, nack the message, requeueing it unless it was redelivered.
     """
 
     def errback(exception: Exception) -> None:
         requeue = not method.redelivered
         logger.exception("Unhandled exception when consuming %r (requeue=%r)", body, requeue)
         nack(state, channel, method.delivery_tag, requeue=requeue)
```

### Comparing `yapw-0.0.9/yapw/methods/blocking.py` & `yapw-0.1.0/yapw/methods.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,87 @@
 """
-Functions for calling channel methods from the context of a consumer callback.
+Functions for calling channel methods from a consumer callback running in another thread.
 """
 
 import functools
 import logging
-from typing import Any, Optional
+from typing import Any
 
 import pika
 
 from yapw.types import State
 from yapw.util import basic_publish_debug_args, basic_publish_kwargs
 
 logger = logging.getLogger(__name__)
 
 
 def publish(
-    state: State, channel: pika.channel.Channel, message: Any, routing_key: str, *args: Any, **kwargs: Any
+    state: State[Any], channel: pika.channel.Channel, message: Any, routing_key: str, *args: Any, **kwargs: Any
 ) -> None:
     """
-    Publish with the provided message and routing key, and with the exchange set by the provided state.
+    Publish the ``message`` with the ``routing_key``, to the exchange set by the ``state``.
 
-    :param state: an object with a ``connection`` attribute
+    :param state: an object with thread-safe attributes from the client
     :param channel: the channel from which to call ``basic_publish``
     :param message: a decoded message
     :param routing_key: the routing key
     """
     keywords = basic_publish_kwargs(state, message, routing_key)
-    keywords.update(kwargs)  # type: ignore # https://github.com/python/mypy/issues/4441
+    keywords.update(kwargs)  # type: ignore # PEP 692 disallows updating TypedDict (PublishKeywords) with Dict.
 
     _channel_method_from_thread(state.connection, channel, "publish", *args, **keywords)
     logger.debug(*basic_publish_debug_args(channel, message, keywords))
 
 
-def ack(state: State, channel: pika.channel.Channel, delivery_tag: Optional[int] = 0, **kwargs: bool) -> None:
+def ack(state: State[Any], channel: pika.channel.Channel, delivery_tag: int | None = 0, **kwargs: bool) -> None:
     """
     Ack a message by its delivery tag.
 
-    :param state: an object with a ``connection`` attribute
+    :param state: an object with thread-safe attributes from the client
     :param channel: the channel from which to call ``basic_ack``
     :param delivery_tag: the delivery tag
     """
     _channel_method_from_thread(state.connection, channel, "ack", delivery_tag, **kwargs)
     logger.debug("Ack'd message on channel %s with delivery tag %s", channel.channel_number, delivery_tag)
 
 
-def nack(state: State, channel: pika.channel.Channel, delivery_tag: Optional[int] = 0, **kwargs: bool) -> None:
+def nack(state: State[Any], channel: pika.channel.Channel, delivery_tag: int | None = 0, **kwargs: bool) -> None:
     """
     Nack a message by its delivery tag.
 
-    :param state: an object with a ``connection`` attribute
+    :param state: an object with thread-safe attributes from the client
     :param channel: the channel from which to call ``basic_nack``
     :param delivery_tag: the delivery tag
     """
     _channel_method_from_thread(state.connection, channel, "nack", delivery_tag, **kwargs)
     logger.debug("Nack'd message on channel %s with delivery tag %s", channel.channel_number, delivery_tag)
 
 
 def _channel_method_from_thread(
-    connection: pika.BlockingConnection, channel: pika.channel.Channel, method: str, *args: Any, **kwargs: Any
+    connection: Any, channel: pika.channel.Channel, method: str, *args: Any, **kwargs: Any
 ) -> None:
     if connection.is_open:
         cb = functools.partial(_channel_method_from_main, channel, method, *args, **kwargs)
-        connection.add_callback_threadsafe(cb)
+        add_callback_threadsafe(connection, cb)
     else:
         logger.error("Can't %s as connection is closed or closing", method)
 
 
 def _channel_method_from_main(channel: pika.channel.Channel, method: str, *args: Any, **kwargs: Any) -> None:
     if channel.is_open:
         getattr(channel, f"basic_{method}")(*args, **kwargs)
     else:
         logger.error("Can't %s as channel is closed or closing", method)
+
+
+def add_callback_threadsafe(connection: Any, callback: Any) -> None:
+    """
+    Interact with Pika from another thread.
+
+    :param connection: a RabbitMQ connection
+    :param callback: the callback to add
+    """
+    # One branch per adapter.
+    if hasattr(connection, "ioloop"):
+        connection.ioloop.call_soon_threadsafe(callback)
+    else:
+        connection.add_callback_threadsafe(callback)
```

### Comparing `yapw-0.0.9/yapw/types.py` & `yapw-0.1.0/yapw/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-import sys
-from typing import Any, Callable, NamedTuple, Optional
+from collections.abc import Callable
+from typing import Any, Generic, NamedTuple, Optional, TypedDict, TypeVar
 
 import pika
 
-if sys.version_info[:2] >= (3, 8):
-    from typing import TypedDict
-else:
-    from typing_extensions import TypedDict  # https://github.com/python/mypy/issues/1153
-
-
-#:
+T = TypeVar("T")
 Encode = Callable[[Any, str], bytes]
-#:
 Decode = Callable[[bytes, Optional[str]], Any]
 
 
-class State(NamedTuple):
+class State(NamedTuple, Generic[T]):
     """
     Attributes that can be used safely in consumer callbacks.
     """
 
     #: A function to format the routing key.
     format_routing_key: Callable[[str], str]
+    #: A function to shut down the client.
+    interrupt: Callable[[T], None]
     #: The connection.
-    connection: pika.BlockingConnection
+    connection: T
     #: The exchange name.
     exchange: str
-    #: The message body's encoder.
+    #: The message bodies' encoder.
     encode: Encode
-    #: The message's content type.
+    #: The messages' content type.
     content_type: str
-    #: The message's delivery mode.
+    #: The messages' delivery mode.
     delivery_mode: int
 
 
 class PublishKeywords(TypedDict, total=False):
     """
     Keyword arguments for ``basic_publish``.
     """
@@ -45,13 +40,11 @@
     routing_key: str
     #: The message's body.
     body: bytes
     #: The message's content type and delivery mode.
     properties: pika.BasicProperties
 
 
-#:
 ConsumerCallback = Callable[[State, pika.channel.Channel, pika.spec.Basic.Deliver, pika.BasicProperties, Any], None]
-#:
 Decorator = Callable[
     [Decode, ConsumerCallback, State, pika.channel.Channel, pika.spec.Basic.Deliver, pika.BasicProperties, bytes], None
 ]
```

### Comparing `yapw-0.0.9/yapw/util.py` & `yapw-0.1.0/yapw/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import json
 import pickle
-from typing import TYPE_CHECKING, Any, Tuple, Union
+from typing import TYPE_CHECKING, Any, Union
 
 import pika
 
 try:
     import orjson
 
     jsonlib = orjson
 except ImportError:
-    jsonlib = json  # type: ignore # https://github.com/python/mypy/issues/1153
+    jsonlib = json  # type: ignore
 
 from yapw.types import PublishKeywords, State
 
 if TYPE_CHECKING:
-    from yapw.clients import Publisher
+    from yapw.clients import Base
 
 
 def json_dumps(message: Any) -> bytes:
     """
     Serialize a Python object to JSON formatted bytes.
 
     Uses `orjson <https://pypi.org/project/orjson/>`__ if available.
@@ -27,14 +27,30 @@
     :returns: JSON formatted bytes
     """
     if jsonlib == json:
         return json.dumps(message, separators=(",", ":")).encode()
     return orjson.dumps(message)
 
 
+def default_decode(body: bytes, content_type: str | None) -> Any:
+    """
+    If the content type is "application/json", deserializes the JSON formatted bytes to a Python object. Otherwise,
+    returns the bytes (which the consumer callback can deserialize independently).
+
+    Uses `orjson <https://pypi.org/project/orjson/>`__ if available.
+
+    :param body: the encoded message
+    :param content_type: the message's content type
+    :returns: a Python object
+    """
+    if content_type == "application/json":
+        return jsonlib.loads(body)
+    return body
+
+
 def default_encode(message: Any, content_type: str) -> bytes:
     """
     Encode the decoded message to bytes.
 
     -  If the content type is "application/json", serialize the message to JSON formatted bytes.
     -  If the message is a string, encode it to bytes.
     -  If the message is bytes, return it.
@@ -49,15 +65,15 @@
     if isinstance(message, str):
         return message.encode()
     if isinstance(message, bytes):
         return message
     return pickle.dumps(message)
 
 
-def basic_publish_kwargs(state: Union["Publisher", State], message: Any, routing_key: str) -> PublishKeywords:
+def basic_publish_kwargs(state: Union["Base[Any]", State[Any]], message: Any, routing_key: str) -> PublishKeywords:
     """
     Prepare keyword arguments for ``basic_publish``.
 
     :param state: an object with the attributes ``format_routing_key``, ``exchange``, ``encode``, ``content_type`` and
                   ``delivery_mode``
     :param message: a decoded message
     :param routing_key: the routing key
@@ -68,16 +84,18 @@
     body = state.encode(message, state.content_type)
     properties = pika.BasicProperties(content_type=state.content_type, delivery_mode=state.delivery_mode)
 
     return {"exchange": state.exchange, "routing_key": formatted, "body": body, "properties": properties}
 
 
 def basic_publish_debug_args(
-    channel: pika.channel.Channel, message: Any, keywords: PublishKeywords
-) -> Tuple[str, Any, int, str, str]:
+    channel: pika.channel.Channel | pika.adapters.blocking_connection.BlockingChannel,
+    message: Any,
+    keywords: PublishKeywords,
+) -> tuple[str, Any, int, str, str]:
     """
     Prepare arguments for ``logger.debug`` related to publishing a message.
 
     :param channel: the channel from which to call ``basic_publish``
     :param message: a decoded message
     :param keywords: keyword arguments for ``basic_publish``
     :returns: arguments for ``logger.debug``
```

### Comparing `yapw-0.0.9/yapw.egg-info/PKG-INFO` & `yapw-0.1.0/yapw.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: yapw
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Pika wrapper with error handling, signal handling and good defaults.
 Home-page: https://github.com/open-contracting/yapw
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: perf
 Provides-Extra: test
 Provides-Extra: types
 Provides-Extra: docs
 License-File: LICENSE
 
 |PyPI Version| |Build Status| |Coverage Status| |Python Version|
 
-Yet Another Pika Wrapper (yapw – pronounced yapu) makes it easier to create a `Pika <https://pika.readthedocs.io/en/stable/>`__ client that has error handling, signal handling, useful logging and good defaults.
+Yet Another Pika Wrapper (yapw – pronounced yapu) makes it easier to create a `Pika <https://pika.readthedocs.io/en/stable/>`__ client that:
+
+-  Runs consumer callbacks in separate threads.
+-  Automatically decodes and encodes messages.
+-  Has error handling, signal handling, useful logging and good defaults.
 
 (If you are viewing this on GitHub, open the `full documentation <https://yapw.readthedocs.io/>`__ for additional details.)
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/yapw.svg
    :target: https://pypi.org/project/yapw/
 .. |Build Status| image:: https://github.com/open-contracting/yapw/workflows/CI/badge.svg
    :target: https://github.com/open-contracting/yapw/actions?query=workflow%3ACI
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/yapw/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/yapw?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/yapw.svg
    :target: https://pypi.org/project/yapw/
-
-
```

### Comparing `yapw-0.0.9/yapw.egg-info/SOURCES.txt` & `yapw-0.1.0/yapw.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
-setup.py
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/api/clients.rst
 docs/api/decorators.rst
 docs/api/index.rst
+docs/api/methods.rst
 docs/api/types.rst
 docs/api/util.rst
-docs/api/methods/blocking.rst
-docs/api/methods/index.rst
 docs/contributing/index.rst
 tests/__init__.py
+tests/conftest.py
 tests/test_decorators.py
+tests/test_methods.py
 tests/test_util.py
 tests/clients/__init__.py
+tests/clients/test_async.py
+tests/clients/test_async_consumer.py
 tests/clients/test_base.py
 tests/clients/test_blocking.py
-tests/clients/test_publisher.py
-tests/clients/test_threaded.py
+tests/clients/test_blocking_consumer.py
+tests/fixtures/busy.py
+tests/fixtures/publisher.py
 tests/fixtures/raiser.py
 tests/fixtures/sleeper.py
-tests/methods/__init__.py
-tests/methods/test_blocking.py
 yapw/__init__.py
 yapw/clients.py
 yapw/decorators.py
+yapw/methods.py
 yapw/ossignal.py
 yapw/py.typed
 yapw/types.py
 yapw/util.py
 yapw.egg-info/PKG-INFO
 yapw.egg-info/SOURCES.txt
 yapw.egg-info/dependency_links.txt
 yapw.egg-info/requires.txt
-yapw.egg-info/top_level.txt
-yapw/methods/__init__.py
-yapw/methods/blocking.py
+yapw.egg-info/top_level.txt
```

