# Comparing `tmp/pydantic-loggings-0.5.0.tar.gz` & `tmp/pydantic-loggings-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-0.5.0.tar", last modified: Mon Jul  3 10:06:11 2023, max compression
+gzip compressed data, was "pydantic-loggings-0.6.0.tar", last modified: Mon Jul  3 10:13:04 2023, max compression
```

## Comparing `pydantic-loggings-0.5.0.tar` & `pydantic-loggings-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     1516 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1195 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1765 2023-07-03 10:05:59.000000 pydantic-loggings-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.095068 pydantic-loggings-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.095068 pydantic-loggings-0.5.0/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/exceptions_.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.095068 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      229 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      639 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/logs.py
--rw-r--r--   0 root         (0) root         (0)     3724 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/mixins.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)      145 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.095068 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1516 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1062 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:13:04.922212 pydantic-loggings-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-03 10:13:04.922212 pydantic-loggings-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-07-03 10:12:52.000000 pydantic-loggings-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 10:13:04.922212 pydantic-loggings-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:13:04.914213 pydantic-loggings-0.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:13:04.918213 pydantic-loggings-0.6.0/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:13:04.918213 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:13:04.918213 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/base/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:13:04.922212 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      639 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/logs.py
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:13:04.918213 pydantic-loggings-0.6.0/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-03 10:13:04.000000 pydantic-loggings-0.6.0/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-07-03 10:13:04.000000 pydantic-loggings-0.6.0/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 10:13:04.000000 pydantic-loggings-0.6.0/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 10:13:04.000000 pydantic-loggings-0.6.0/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 10:13:04.000000 pydantic-loggings-0.6.0/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:13:04.922212 pydantic-loggings-0.6.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-03 10:12:51.000000 pydantic-loggings-0.6.0/tests/test_main.py
```

### Comparing `pydantic-loggings-0.5.0/PKG-INFO` & `pydantic-loggings-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.5.0
+Version: 0.6.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Configure Python logging from environment variables with pydantic (settings) Model
```

### Comparing `pydantic-loggings-0.5.0/README.md` & `pydantic-loggings-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.5.0/pyproject.toml` & `pydantic-loggings-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 authors = [
   {name = "m9810223", email = "m9810223@gmail.com"},
 ]
 name = "pydantic-loggings"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "0.5.0"
+version = "0.6.0"
 
 dependencies = [
   "pydantic>=2.0",
   "pydantic-settings>=2.0",
 ]
 
 [project.urls]
```

### Comparing `pydantic-loggings-0.5.0/src/pydantic_loggings/__init__.py` & `pydantic-loggings-0.6.0/src/pydantic_loggings/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/logs.py` & `pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/base/logs.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/formatters.py` & `pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/handlers.py` & `pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/loggers.py` & `pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/logs.py` & `pydantic-loggings-0.6.0/src/pydantic_loggings/loggings/not_set/logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import typing as t
+import warnings
 from logging.config import DictConfigurator
 
 from pydantic_settings import BaseSettings
 from pydantic_settings import SettingsConfigDict
 
-from ... import exceptions_
 from ... import mixins
 from .filters import Filter
 from .formatters import Formatter
 from .handlers import Handler
 from .loggers import Logger
 
 
@@ -46,13 +46,13 @@
         self._configure(configuration)
 
     def is_valid_logger_name(self, logger_name: str):
         return logger_name in ['', 'root', *(self.loggers or {}).keys()]
 
     def get_logger(self, logger_name: str):
         if not self.is_valid_logger_name(logger_name):
-            raise exceptions_.LoggerNotFoundError(logger_name)
+            warnings.warn(f'Logger: `{logger_name}` is not found.')
         return logging.getLogger(name=logger_name)
 
     def configure_and_get_logger(self, logger_name: str = ''):
         self.configure()
         return self.get_logger(logger_name=logger_name)
```

### Comparing `pydantic-loggings-0.5.0/src/pydantic_loggings/mixins.py` & `pydantic-loggings-0.6.0/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-0.6.0/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.5.0
+Version: 0.6.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Configure Python logging from environment variables with pydantic (settings) Model
```

### Comparing `pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-0.6.0/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 pyproject.toml
 src/pydantic_loggings/__init__.py
-src/pydantic_loggings/exceptions_.py
 src/pydantic_loggings/mixins.py
 src/pydantic_loggings/types_.py
 src/pydantic_loggings/utils.py
 src/pydantic_loggings.egg-info/PKG-INFO
 src/pydantic_loggings.egg-info/SOURCES.txt
 src/pydantic_loggings.egg-info/dependency_links.txt
 src/pydantic_loggings.egg-info/requires.txt
```

