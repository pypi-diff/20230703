# Comparing `tmp/irc_api-1.0.0.tar.gz` & `tmp/irc_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-1.0.0.tar", last modified: Sun Jul  2 13:21:58 2023, max compression
+gzip compressed data, was "irc_api-1.0.1.tar", last modified: Mon Jul  3 15:00:52 2023, max compression
```

## Comparing `irc_api-1.0.0.tar` & `irc_api-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:21:58.490130 irc_api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 13:21:44.000000 irc_api-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-02 13:21:58.490130 irc_api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-02 13:21:44.000000 irc_api-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-02 13:21:44.000000 irc_api-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:21:58.490130 irc_api-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:21:58.490130 irc_api-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:21:58.490130 irc_api-1.0.0/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:21:58.490130 irc_api-1.0.0/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:00:52.572323 irc_api-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 15:00:41.000000 irc_api-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-03 15:00:52.572323 irc_api-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 15:00:41.000000 irc_api-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-03 15:00:41.000000 irc_api-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:00:52.572323 irc_api-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:00:52.568323 irc_api-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:00:52.572323 irc_api-1.0.1/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-03 15:00:41.000000 irc_api-1.0.1/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:00:52.572323 irc_api-1.0.1/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 15:00:52.000000 irc_api-1.0.1/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-1.0.0/LICENSE` & `irc_api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.0/PKG-INFO` & `irc_api-1.0.1/src/irc_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: irc_api
-Version: 1.0.0
+Name: irc-api
+Version: 1.0.1
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # IRC API
-[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/github/license/Shadow15510/irc_api?color=green)](https://github.com/Shadow15510/irc_api/blob/master/LICENSE)
 
 ## Description
 IRC API is a small API to make Python IRC bots. This API is based on decorators to make commands like the `cog` module in `discord.py`.
 
 If you encounter any issue feel free to [open one](https://github.com/Shadow15510/irc_api/issues).
 A full documentation is available on [readthedocs](https://irc-api.readthedocs.io/en/latest/).
```

### Comparing `irc_api-1.0.0/README.md` & `irc_api-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # IRC API
-[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/github/license/Shadow15510/irc_api?color=green)](https://github.com/Shadow15510/irc_api/blob/master/LICENSE)
 
 ## Description
 IRC API is a small API to make Python IRC bots. This API is based on decorators to make commands like the `cog` module in `discord.py`.
 
 If you encounter any issue feel free to [open one](https://github.com/Shadow15510/irc_api/issues).
 A full documentation is available on [readthedocs](https://irc-api.readthedocs.io/en/latest/).
```

### Comparing `irc_api-1.0.0/pyproject.toml` & `irc_api-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 [project]
 name = "irc_api"
 authors = [
 	{name="Sha-chan"},
 ]
 description = "An API written in Python to make IRC bots."
-readme = "README.md"
+readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 	"Development Status :: 5 - Production/Stable",
 ]
-
 dynamic = [
 	"version",
 ]
 
 [tool.setuptools]
 license-files = [
     "LICENSE",
```

### Comparing `irc_api-1.0.0/src/irc_api/bot.py` & `irc_api-1.0.1/src/irc_api/bot.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.0/src/irc_api/commands.py` & `irc_api-1.0.1/src/irc_api/commands.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.0/src/irc_api/history.py` & `irc_api-1.0.1/src/irc_api/history.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.0/src/irc_api/irc.py` & `irc_api-1.0.1/src/irc_api/irc.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.0/src/irc_api/message.py` & `irc_api-1.0.1/src/irc_api/message.py`

 * *Files identical despite different names*

### Comparing `irc_api-1.0.0/src/irc_api.egg-info/PKG-INFO` & `irc_api-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: irc-api
-Version: 1.0.0
+Name: irc_api
+Version: 1.0.1
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # IRC API
-[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest) [![Licence](https://img.shields.io/github/license/Shadow15510/irc_api?color=green)](https://github.com/Shadow15510/irc_api/blob/master/LICENSE)
 
 ## Description
 IRC API is a small API to make Python IRC bots. This API is based on decorators to make commands like the `cog` module in `discord.py`.
 
 If you encounter any issue feel free to [open one](https://github.com/Shadow15510/irc_api/issues).
 A full documentation is available on [readthedocs](https://irc-api.readthedocs.io/en/latest/).
```

