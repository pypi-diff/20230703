# Comparing `tmp/hspylib-cfman-0.9.91.tar.gz` & `tmp/hspylib-cfman-0.9.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-cfman-0.9.91.tar", last modified: Tue Jun 27 22:01:07 2023, max compression
+gzip compressed data, was "hspylib-cfman-0.9.92.tar", last modified: Mon Jul  3 19:09:01 2023, max compression
```

## Comparing `hspylib-cfman-0.9.91.tar` & `hspylib-cfman-0.9.92.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-06-27 22:01:07.102869 hspylib-cfman-0.9.91/
--rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.91/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-06-27 22:01:07.101518 hspylib-cfman-0.9.91/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-06-27 22:01:07.074968 hspylib-cfman-0.9.91/cfman/
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/cfman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.91/cfman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/cfman/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3472 2023-06-27 21:55:04.000000 hspylib-cfman-0.9.91/cfman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-06-27 22:01:07.086120 hspylib-cfman-0.9.91/cfman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/cfman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7745 2023-06-27 21:59:43.000000 hspylib-cfman-0.9.91/cfman/core/cf.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2950 2023-05-17 21:37:29.000000 hspylib-cfman-0.9.91/cfman/core/cf_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5534 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.91/cfman/core/cf_blue_green_checker.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1234 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.91/cfman/core/cf_endpoint.py
--rw-r--r--   0 hjunior    (504) staff       (20)    16928 2023-06-27 21:59:31.000000 hspylib-cfman-0.9.91/cfman/core/cf_manager.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-06-27 22:01:07.090829 hspylib-cfman-0.9.91/cfman/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/cfman/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.91/cfman/exception/exceptions.py
--rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.91/cfman/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-06-27 22:01:07.099666 hspylib-cfman-0.9.91/hspylib_cfman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/hspylib_cfman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/hspylib_cfman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/hspylib_cfman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/hspylib_cfman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-06-27 22:01:06.000000 hspylib-cfman-0.9.91/hspylib_cfman.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-06-27 22:01:07.103095 hspylib-cfman-0.9.91/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1934 2023-04-19 22:13:46.000000 hspylib-cfman-0.9.91/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:09:01.932502 hspylib-cfman-0.9.92/
+-rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.92/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-03 19:09:01.931187 hspylib-cfman-0.9.92/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-07-03 19:09:00.000000 hspylib-cfman-0.9.92/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:09:01.901412 hspylib-cfman-0.9.92/cfman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-03 19:09:00.000000 hspylib-cfman-0.9.92/cfman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.92/cfman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-03 19:09:00.000000 hspylib-cfman-0.9.92/cfman/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3472 2023-06-27 21:55:04.000000 hspylib-cfman-0.9.92/cfman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:09:01.913511 hspylib-cfman-0.9.92/cfman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-07-03 19:09:00.000000 hspylib-cfman-0.9.92/cfman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7745 2023-06-27 21:59:43.000000 hspylib-cfman-0.9.92/cfman/core/cf.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2950 2023-05-17 21:37:29.000000 hspylib-cfman-0.9.92/cfman/core/cf_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5534 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.92/cfman/core/cf_blue_green_checker.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1234 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.92/cfman/core/cf_endpoint.py
+-rw-r--r--   0 hjunior    (504) staff       (20)    16928 2023-06-27 21:59:31.000000 hspylib-cfman-0.9.92/cfman/core/cf_manager.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:09:01.918789 hspylib-cfman-0.9.92/cfman/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-03 19:09:00.000000 hspylib-cfman-0.9.92/cfman/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.92/cfman/exception/exceptions.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.92/cfman/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:09:01.929129 hspylib-cfman-0.9.92/hspylib_cfman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-03 19:09:01.000000 hspylib-cfman-0.9.92/hspylib_cfman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-07-03 19:09:01.000000 hspylib-cfman-0.9.92/hspylib_cfman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-03 19:09:01.000000 hspylib-cfman-0.9.92/hspylib_cfman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-07-03 19:09:01.000000 hspylib-cfman-0.9.92/hspylib_cfman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-03 19:09:01.000000 hspylib-cfman-0.9.92/hspylib_cfman.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-03 19:09:01.932701 hspylib-cfman-0.9.92/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1934 2023-04-19 22:13:46.000000 hspylib-cfman-0.9.92/setup.py
```

### Comparing `hspylib-cfman-0.9.91/PKG-INFO` & `hspylib-cfman-0.9.92/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.91
+Version: 0.9.92
 Summary: HsPyLib - CloudFoundry manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-cfman/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - CloudFoundry manager
 
 ## Manage your PCF applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.91/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.92/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.91/README.md` & `hspylib-cfman-0.9.92/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - CloudFoundry manager
 
 ## Manage your PCF applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.91/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.92/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.91/cfman/__classpath__.py` & `hspylib-cfman-0.9.92/cfman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.91/cfman/__main__.py` & `hspylib-cfman-0.9.92/cfman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.91/cfman/core/cf.py` & `hspylib-cfman-0.9.92/cfman/core/cf.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.91/cfman/core/cf_application.py` & `hspylib-cfman-0.9.92/cfman/core/cf_application.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.91/cfman/core/cf_blue_green_checker.py` & `hspylib-cfman-0.9.92/cfman/core/cf_blue_green_checker.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.91/cfman/core/cf_endpoint.py` & `hspylib-cfman-0.9.92/cfman/core/cf_endpoint.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.91/cfman/core/cf_manager.py` & `hspylib-cfman-0.9.92/cfman/core/cf_manager.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.91/cfman/exception/exceptions.py` & `hspylib-cfman-0.9.92/cfman/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.91/hspylib_cfman.egg-info/PKG-INFO` & `hspylib-cfman-0.9.92/hspylib_cfman.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.91
+Version: 0.9.92
 Summary: HsPyLib - CloudFoundry manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-cfman/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - CloudFoundry manager
 
 ## Manage your PCF applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.91/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.92/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.91/hspylib_cfman.egg-info/SOURCES.txt` & `hspylib-cfman-0.9.92/hspylib_cfman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.91/setup.py` & `hspylib-cfman-0.9.92/setup.py`

 * *Files identical despite different names*

