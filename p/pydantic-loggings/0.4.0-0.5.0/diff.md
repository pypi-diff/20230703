# Comparing `tmp/pydantic-loggings-0.4.0.tar.gz` & `tmp/pydantic-loggings-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-0.4.0.tar", last modified: Mon Jul  3 10:02:56 2023, max compression
+gzip compressed data, was "pydantic-loggings-0.5.0.tar", last modified: Mon Jul  3 10:06:11 2023, max compression
```

## Comparing `pydantic-loggings-0.4.0.tar` & `pydantic-loggings-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:02:56.870953 pydantic-loggings-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1501 2023-07-03 10:02:56.870953 pydantic-loggings-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1180 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1765 2023-07-03 10:02:44.000000 pydantic-loggings-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 10:02:56.870953 pydantic-loggings-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:02:56.866953 pydantic-loggings-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:02:56.866953 pydantic-loggings-0.4.0/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)      580 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/exceptions_.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:02:56.866953 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:02:56.870953 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/base/
--rw-r--r--   0 root         (0) root         (0)      269 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/base/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:02:56.870953 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      229 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      639 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/logs.py
--rw-r--r--   0 root         (0) root         (0)     3724 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/mixins.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)      145 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:02:56.866953 pydantic-loggings-0.4.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1501 2023-07-03 10:02:56.000000 pydantic-loggings-0.4.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1062 2023-07-03 10:02:56.000000 pydantic-loggings-0.4.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 10:02:56.000000 pydantic-loggings-0.4.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 10:02:56.000000 pydantic-loggings-0.4.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 10:02:56.000000 pydantic-loggings-0.4.0/src/pydantic_loggings.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:02:56.870953 pydantic-loggings-0.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-03 10:02:43.000000 pydantic-loggings-0.4.0/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-07-03 10:05:59.000000 pydantic-loggings-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.095068 pydantic-loggings-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.095068 pydantic-loggings-0.5.0/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/exceptions_.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.095068 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      639 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/logs.py
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/mixins.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.095068 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-03 10:06:11.000000 pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 10:06:11.099069 pydantic-loggings-0.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-03 10:05:58.000000 pydantic-loggings-0.5.0/tests/test_main.py
```

### Comparing `pydantic-loggings-0.4.0/PKG-INFO` & `pydantic-loggings-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.4.0
+Version: 0.5.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Configure Python logging from environment variables with pydantic (settings) Model
@@ -29,33 +29,33 @@
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
 # 01-01 00:00:00 WARNING root warning
 ```
 
-### from `.env` file
+### from env file
 
 ```shell
-# ./.env
+# ./log.conf.env
 log__formatters__base__datefmt='%m-%dT%X'
 log__formatters__base__format='{asctime} {levelname:5} {name} {message}'
 log__formatters__base__style='{'
 
 log__handlers__base__class_='logging.StreamHandler'
 log__handlers__base__formatter='base'
 
 log__loggers__root__level='DEBUG'
 log__loggers__root__handlers='["base"]'
 ```
 
 ```py
 from pydantic_loggings import Log
 
-logger = Log(_env_file='.env').configure_and_get_logger()
+logger = Log(_env_file='./log.conf.env').configure_and_get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
```

### Comparing `pydantic-loggings-0.4.0/README.md` & `pydantic-loggings-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
 # 01-01 00:00:00 WARNING root warning
 ```
 
-### from `.env` file
+### from env file
 
 ```shell
-# ./.env
+# ./log.conf.env
 log__formatters__base__datefmt='%m-%dT%X'
 log__formatters__base__format='{asctime} {levelname:5} {name} {message}'
 log__formatters__base__style='{'
 
 log__handlers__base__class_='logging.StreamHandler'
 log__handlers__base__formatter='base'
 
 log__loggers__root__level='DEBUG'
 log__loggers__root__handlers='["base"]'
 ```
 
 ```py
 from pydantic_loggings import Log
 
-logger = Log(_env_file='.env').configure_and_get_logger()
+logger = Log(_env_file='./log.conf.env').configure_and_get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
```

### Comparing `pydantic-loggings-0.4.0/pyproject.toml` & `pydantic-loggings-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 authors = [
   {name = "m9810223", email = "m9810223@gmail.com"},
 ]
 name = "pydantic-loggings"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "0.4.0"
+version = "0.5.0"
 
 dependencies = [
   "pydantic>=2.0",
   "pydantic-settings>=2.0",
 ]
 
 [project.urls]
```

### Comparing `pydantic-loggings-0.4.0/src/pydantic_loggings/__init__.py` & `pydantic-loggings-0.5.0/src/pydantic_loggings/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/base/logs.py` & `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/base/logs.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/formatters.py` & `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/handlers.py` & `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/loggers.py` & `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.4.0/src/pydantic_loggings/loggings/not_set/logs.py` & `pydantic-loggings-0.5.0/src/pydantic_loggings/loggings/not_set/logs.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.4.0/src/pydantic_loggings/mixins.py` & `pydantic-loggings-0.5.0/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.4.0/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.4.0
+Version: 0.5.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Configure Python logging from environment variables with pydantic (settings) Model
@@ -29,33 +29,33 @@
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
 # 01-01 00:00:00 WARNING root warning
 ```
 
-### from `.env` file
+### from env file
 
 ```shell
-# ./.env
+# ./log.conf.env
 log__formatters__base__datefmt='%m-%dT%X'
 log__formatters__base__format='{asctime} {levelname:5} {name} {message}'
 log__formatters__base__style='{'
 
 log__handlers__base__class_='logging.StreamHandler'
 log__handlers__base__formatter='base'
 
 log__loggers__root__level='DEBUG'
 log__loggers__root__handlers='["base"]'
 ```
 
 ```py
 from pydantic_loggings import Log
 
-logger = Log(_env_file='.env').configure_and_get_logger()
+logger = Log(_env_file='./log.conf.env').configure_and_get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG root debug
 # 01-01 00:00:00 INFO  root info
```

### Comparing `pydantic-loggings-0.4.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-0.5.0/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

