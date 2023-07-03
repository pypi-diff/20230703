# Comparing `tmp/hspylib-hqt-0.9.3.tar.gz` & `tmp/hspylib-hqt-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-hqt-0.9.3.tar", last modified: Fri May 19 18:16:19 2023, max compression
+gzip compressed data, was "hspylib-hqt-0.9.4.tar", last modified: Mon Jul  3 19:10:01 2023, max compression
```

## Comparing `hspylib-hqt-0.9.3.tar` & `hspylib-hqt-0.9.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.906880 hspylib-hqt-0.9.3/
--rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.3/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)    11723 2023-05-19 18:16:19.905577 hspylib-hqt-0.9.3/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)    10711 2023-05-19 18:16:18.000000 hspylib-hqt-0.9.3/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.872965 hspylib-hqt-0.9.3/hqt/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-05-19 18:16:18.000000 hspylib-hqt-0.9.3/hqt/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      198 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hqt/__init__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.887851 hspylib-hqt-0.9.3/hqt/promotions/
--rw-r--r--   0 hjunior    (504) staff       (20)      284 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hqt/promotions/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      838 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hcombobox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7680 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hconsole.py
--rw-r--r--   0 hjunior    (504) staff       (20)      667 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hframe.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2570 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hlabel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6562 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hlistwidget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4414 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/hstacked_widget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6227 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/htablemodel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5448 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/htableview.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6283 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/promotions/htoolbox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2592 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/qt_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3854 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/stream_capturer.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.894111 hspylib-hqt-0.9.3/hqt/views/
--rw-r--r--   0 hjunior    (504) staff       (20)      162 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hqt/views/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      862 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/views/main_view.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2313 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.3/hqt/views/qt_view.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-05-19 18:16:19.903988 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)    11723 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       26 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        4 2023-05-19 18:16:19.000000 hspylib-hqt-0.9.3/hspylib_hqt.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-05-19 18:16:19.907110 hspylib-hqt-0.9.3/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2071 2023-04-19 22:12:01.000000 hspylib-hqt-0.9.3/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:10:01.386098 hspylib-hqt-0.9.4/
+-rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.4/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-03 19:10:01.384948 hspylib-hqt-0.9.4/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)    11082 2023-07-03 19:10:00.000000 hspylib-hqt-0.9.4/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:10:01.350495 hspylib-hqt-0.9.4/hqt/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-03 19:10:00.000000 hspylib-hqt-0.9.4/hqt/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      198 2023-07-03 19:10:00.000000 hspylib-hqt-0.9.4/hqt/__init__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:10:01.367263 hspylib-hqt-0.9.4/hqt/promotions/
+-rw-r--r--   0 hjunior    (504) staff       (20)      284 2023-07-03 19:10:00.000000 hspylib-hqt-0.9.4/hqt/promotions/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      838 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/promotions/hcombobox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7680 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/promotions/hconsole.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      667 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/promotions/hframe.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2570 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/promotions/hlabel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6562 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/promotions/hlistwidget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4414 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/promotions/hstacked_widget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6227 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/promotions/htablemodel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5448 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/promotions/htableview.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6283 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/promotions/htoolbox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2592 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/qt_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3854 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/stream_capturer.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:10:01.374321 hspylib-hqt-0.9.4/hqt/views/
+-rw-r--r--   0 hjunior    (504) staff       (20)      162 2023-07-03 19:10:00.000000 hspylib-hqt-0.9.4/hqt/views/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      862 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/views/main_view.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2313 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.4/hqt/views/qt_view.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 19:10:01.383595 hspylib-hqt-0.9.4/hspylib_hqt.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-03 19:10:01.000000 hspylib-hqt-0.9.4/hspylib_hqt.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-07-03 19:10:01.000000 hspylib-hqt-0.9.4/hspylib_hqt.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-03 19:10:01.000000 hspylib-hqt-0.9.4/hspylib_hqt.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       26 2023-07-03 19:10:01.000000 hspylib-hqt-0.9.4/hspylib_hqt.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        4 2023-07-03 19:10:01.000000 hspylib-hqt-0.9.4/hspylib_hqt.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-03 19:10:01.386272 hspylib-hqt-0.9.4/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2071 2023-04-19 22:12:01.000000 hspylib-hqt-0.9.4/setup.py
```

### Comparing `hspylib-hqt-0.9.3/PKG-INFO` & `hspylib-hqt-0.9.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-hqt
-Version: 0.9.3
+Version: 0.9.4
 Summary: HsPyLib - QT framework extensions
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-hqt/
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 
 # <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
 ## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.3/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.4/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
@@ -330,14 +330,24 @@
 You can support HsPyLib
 by [donating](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 or coding. Fell free to contact me for details. When contributing with code change please take a look at our
 [guidelines](docs/CONTRIBUTING.md) and [code of conduct](docs/CODE_OF_CONDUCT.md).
 
 [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
+## Sponsors
+
+This project is supported by:
+
+<a href="https://www.jetbrains.com/community/opensource/?utm_campaign=opensource&utm_content=approved&utm_medium=email&utm_source=newsletter&utm_term=jblogo#support">
+  <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" width="120" height="120">
+</a>
+
+Thank you for your support <3 !!
+
 ## Links
 
 - Documentation: [API](docs/api/index.html)
 - License: [MIT](LICENSE.md)
 - Releases: https://pypi.org/project/hspylib/#history
 - Code: https://github.com/yorevs/hspylib
 - Issue tracker: https://github.com/yorevs/hspylib/issues
```

### Comparing `hspylib-hqt-0.9.3/README.md` & `hspylib-hqt-0.9.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
 ## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.3/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.4/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
@@ -303,14 +303,24 @@
 You can support HsPyLib
 by [donating](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 or coding. Fell free to contact me for details. When contributing with code change please take a look at our
 [guidelines](docs/CONTRIBUTING.md) and [code of conduct](docs/CODE_OF_CONDUCT.md).
 
 [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
+## Sponsors
+
+This project is supported by:
+
+<a href="https://www.jetbrains.com/community/opensource/?utm_campaign=opensource&utm_content=approved&utm_medium=email&utm_source=newsletter&utm_term=jblogo#support">
+  <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" width="120" height="120">
+</a>
+
+Thank you for your support <3 !!
+
 ## Links
 
 - Documentation: [API](docs/api/index.html)
 - License: [MIT](LICENSE.md)
 - Releases: https://pypi.org/project/hspylib/#history
 - Code: https://github.com/yorevs/hspylib
 - Issue tracker: https://github.com/yorevs/hspylib/issues
```

### Comparing `hspylib-hqt-0.9.3/hqt/promotions/hcombobox.py` & `hspylib-hqt-0.9.4/hqt/promotions/hcombobox.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/promotions/hconsole.py` & `hspylib-hqt-0.9.4/hqt/promotions/hconsole.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/promotions/hframe.py` & `hspylib-hqt-0.9.4/hqt/promotions/hframe.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/promotions/hlabel.py` & `hspylib-hqt-0.9.4/hqt/promotions/hlabel.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/promotions/hlistwidget.py` & `hspylib-hqt-0.9.4/hqt/promotions/hlistwidget.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/promotions/hstacked_widget.py` & `hspylib-hqt-0.9.4/hqt/promotions/hstacked_widget.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/promotions/htablemodel.py` & `hspylib-hqt-0.9.4/hqt/promotions/htablemodel.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/promotions/htableview.py` & `hspylib-hqt-0.9.4/hqt/promotions/htableview.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/promotions/htoolbox.py` & `hspylib-hqt-0.9.4/hqt/promotions/htoolbox.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/qt_application.py` & `hspylib-hqt-0.9.4/hqt/qt_application.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/stream_capturer.py` & `hspylib-hqt-0.9.4/hqt/stream_capturer.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/views/main_view.py` & `hspylib-hqt-0.9.4/hqt/views/main_view.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hqt/views/qt_view.py` & `hspylib-hqt-0.9.4/hqt/views/qt_view.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/hspylib_hqt.egg-info/PKG-INFO` & `hspylib-hqt-0.9.4/hspylib_hqt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-hqt
-Version: 0.9.3
+Version: 0.9.4
 Summary: HsPyLib - QT framework extensions
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-hqt/
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 
 # <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
 ## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.3/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.4/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
@@ -330,14 +330,24 @@
 You can support HsPyLib
 by [donating](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 or coding. Fell free to contact me for details. When contributing with code change please take a look at our
 [guidelines](docs/CONTRIBUTING.md) and [code of conduct](docs/CODE_OF_CONDUCT.md).
 
 [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
+## Sponsors
+
+This project is supported by:
+
+<a href="https://www.jetbrains.com/community/opensource/?utm_campaign=opensource&utm_content=approved&utm_medium=email&utm_source=newsletter&utm_term=jblogo#support">
+  <img src="https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.png" width="120" height="120">
+</a>
+
+Thank you for your support <3 !!
+
 ## Links
 
 - Documentation: [API](docs/api/index.html)
 - License: [MIT](LICENSE.md)
 - Releases: https://pypi.org/project/hspylib/#history
 - Code: https://github.com/yorevs/hspylib
 - Issue tracker: https://github.com/yorevs/hspylib/issues
```

### Comparing `hspylib-hqt-0.9.3/hspylib_hqt.egg-info/SOURCES.txt` & `hspylib-hqt-0.9.4/hspylib_hqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.3/setup.py` & `hspylib-hqt-0.9.4/setup.py`

 * *Files identical despite different names*

