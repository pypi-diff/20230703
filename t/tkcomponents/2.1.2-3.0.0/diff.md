# Comparing `tmp/tkcomponents-2.1.2.tar.gz` & `tmp/tkcomponents-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkcomponents-2.1.2.tar", last modified: Sat Jun 24 05:09:47 2023, max compression
+gzip compressed data, was "tkcomponents-3.0.0.tar", last modified: Mon Jul  3 04:49:04 2023, max compression
```

## Comparing `tkcomponents-2.1.2.tar` & `tkcomponents-3.0.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.371451 tkcomponents-2.1.2/
--rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-2.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-2.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-06-24 05:09:47.371451 tkcomponents-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-2.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 05:09:47.371451 tkcomponents-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-06-24 05:09:13.000000 tkcomponents-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.320440 tkcomponents-2.1.2/tkcomponents/
--rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-2.1.2/tkcomponents/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.345421 tkcomponents-2.1.2/tkcomponents/abstractcomponents/
--rw-rw-rw-   0        0        0       90 2021-02-08 14:22:06.000000 tkcomponents-2.1.2/tkcomponents/abstractcomponents/__init__.py
--rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/abstractcomponents/timedframe.py
--rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/abstractcomponents/verticalscrollframe.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.356421 tkcomponents-2.1.2/tkcomponents/basiccomponents/
--rw-rw-rw-   0        0        0      472 2021-10-01 23:21:42.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/__init__.py
--rw-rw-rw-   0        0        0     1612 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/alert.py
--rw-rw-rw-   0        0        0     2322 2021-11-02 01:05:45.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/buttonlistbox.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.368451 tkcomponents-2.1.2/tkcomponents/basiccomponents/classes/
--rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/classes/dateticker.py
--rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/classes/timer.py
--rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/constants.py
--rw-rw-rw-   0        0        0     3068 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/datestepper.py
--rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/labelwrapper.py
--rw-rw-rw-   0        0        0     4981 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/numberstepper.py
--rw-rw-rw-   0        0        0     2568 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/numbersteppertable.py
--rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/progressbar.py
--rw-rw-rw-   0        0        0     2861 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/stringeditor.py
--rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/textcarousel.py
--rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/timercontrol.py
--rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-2.1.2/tkcomponents/basiccomponents/togglebutton.py
--rw-rw-rw-   0        0        0     7621 2022-02-25 14:08:12.000000 tkcomponents-2.1.2/tkcomponents/component.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.370421 tkcomponents-2.1.2/tkcomponents/extensions/
--rw-rw-rw-   0        0        0       36 2021-02-08 12:20:34.000000 tkcomponents-2.1.2/tkcomponents/extensions/__init__.py
--rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-2.1.2/tkcomponents/extensions/gridhelper.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:09:47.342451 tkcomponents-2.1.2/tkcomponents.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-24 05:09:47.000000 tkcomponents-2.1.2/tkcomponents.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.185560 tkcomponents-3.0.0/
+-rw-rw-rw-   0        0        0     1087 2021-02-07 14:49:35.000000 tkcomponents-3.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       40 2021-02-07 14:36:16.000000 tkcomponents-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-03 04:49:04.185560 tkcomponents-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2022-02-25 13:47:36.000000 tkcomponents-3.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 04:49:04.186560 tkcomponents-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2023-07-03 04:47:52.000000 tkcomponents-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.132562 tkcomponents-3.0.0/tkcomponents/
+-rw-rw-rw-   0        0        0       34 2020-11-29 03:48:50.000000 tkcomponents-3.0.0/tkcomponents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.169561 tkcomponents-3.0.0/tkcomponents/basiccomponents/
+-rw-rw-rw-   0        0        0      564 2023-07-02 09:02:35.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/__init__.py
+-rw-rw-rw-   0        0        0     1592 2023-06-28 05:29:47.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/alert.py
+-rw-rw-rw-   0        0        0     2302 2023-06-28 05:29:47.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/buttonlistbox.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.182560 tkcomponents-3.0.0/tkcomponents/basiccomponents/classes/
+-rw-rw-rw-   0        0        0      338 2020-11-18 00:08:16.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/classes/dateticker.py
+-rw-rw-rw-   0        0        0     1175 2021-02-09 06:25:11.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/classes/timer.py
+-rw-rw-rw-   0        0        0      203 2020-12-25 08:29:15.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/constants.py
+-rw-rw-rw-   0        0        0     3068 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/datestepper.py
+-rw-rw-rw-   0        0        0      850 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/labelwrapper.py
+-rw-rw-rw-   0        0        0     4981 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/numberstepper.py
+-rw-rw-rw-   0        0        0     2568 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/numbersteppertable.py
+-rw-rw-rw-   0        0        0     3577 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/progressbar.py
+-rw-rw-rw-   0        0        0     2861 2023-07-03 00:51:53.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/stringeditor.py
+-rw-rw-rw-   0        0        0     3259 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/textcarousel.py
+-rw-rw-rw-   0        0        0     2180 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/timedframe.py
+-rw-rw-rw-   0        0        0     2743 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/timercontrol.py
+-rw-rw-rw-   0        0        0     1575 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/togglebutton.py
+-rw-rw-rw-   0        0        0     3018 2022-02-25 14:01:02.000000 tkcomponents-3.0.0/tkcomponents/basiccomponents/verticalscrollframe.py
+-rw-rw-rw-   0        0        0     7621 2023-07-01 02:53:52.000000 tkcomponents-3.0.0/tkcomponents/component.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.184561 tkcomponents-3.0.0/tkcomponents/extensions/
+-rw-rw-rw-   0        0        0       74 2023-07-02 09:02:34.000000 tkcomponents-3.0.0/tkcomponents/extensions/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-07-02 09:11:53.000000 tkcomponents-3.0.0/tkcomponents/extensions/draganddrop.py
+-rw-rw-rw-   0        0        0     1590 2022-07-20 00:30:12.000000 tkcomponents-3.0.0/tkcomponents/extensions/gridhelper.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:49:04.155562 tkcomponents-3.0.0/tkcomponents.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1154 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 04:49:04.000000 tkcomponents-3.0.0/tkcomponents.egg-info/top_level.txt
```

### Comparing `tkcomponents-2.1.2/LICENSE.txt` & `tkcomponents-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/PKG-INFO` & `tkcomponents-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 2.1.2
+Version: 3.0.0
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v2.1.2.tar.gz
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v3.0.0.tar.gz
 Author: immijimmi
 Author-email: immijimmi1@gmail.com
 License: MIT
 Keywords: ui,gui,graphical,user,interface
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `tkcomponents-2.1.2/README.md` & `tkcomponents-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/setup.py` & `tkcomponents-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 with open("README.md", "r", encoding="utf-8") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="tkcomponents",
     packages=[
-        "tkcomponents", "tkcomponents.extensions", "tkcomponents.basiccomponents", "tkcomponents.abstractcomponents",
+        "tkcomponents", "tkcomponents.extensions", "tkcomponents.basiccomponents",
         "tkcomponents.basiccomponents.classes"
     ],
-    version="2.1.2",
+    version="3.0.0",
     license="MIT",
     description="An OOP framework for Tkinter, inspired by React",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="immijimmi",
     author_email="immijimmi1@gmail.com",
     url="https://github.com/immijimmi/tkcomponents",
-    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v2.1.2.tar.gz",
+    download_url="https://github.com/immijimmi/tkcomponents/archive/refs/tags/v3.0.0.tar.gz",
     keywords=[
         'ui', 'gui', 'graphical', 'user', 'interface'
     ],
     install_requires=[
         'objectextensions~=2.0.2'
     ],
     classifiers=[
```

### Comparing `tkcomponents-2.1.2/tkcomponents/abstractcomponents/timedframe.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/timedframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/abstractcomponents/verticalscrollframe.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/verticalscrollframe.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/alert.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/alert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tkinter import StringVar, Label, Button
 
 from ..extensions import GridHelper
-from ..abstractcomponents.timedframe import TimedFrame
+from .timedframe import TimedFrame
 from .constants import Constants
 
 
 class Alert(TimedFrame.with_extensions(GridHelper)):
     def __init__(self, container, duration, get_data, on_expire=lambda alert: None, update_interval_ms=None, styles=None):
         super().__init__(container, duration, on_expire=on_expire, get_data=get_data,
                          update_interval_ms=update_interval_ms, styles=styles)
```

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/buttonlistbox.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/buttonlistbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tkinter import Button
 from functools import partial
 
-from ..abstractcomponents.verticalscrollframe import VerticalScrollFrame
+from .verticalscrollframe import VerticalScrollFrame
 
 
 class ButtonListBox(VerticalScrollFrame):
     def __init__(self, container, current_value, get_height,
                  get_data, on_change=(lambda picker, new_value: None), styles=None):
         super().__init__(container, get_height,
                          get_data=get_data, on_change=on_change, styles=styles)
```

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/classes/timer.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/classes/timer.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/datestepper.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/datestepper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/labelwrapper.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/labelwrapper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/numberstepper.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/numberstepper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/numbersteppertable.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/numbersteppertable.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/progressbar.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/progressbar.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/stringeditor.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/stringeditor.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/textcarousel.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/textcarousel.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/timercontrol.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/timercontrol.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/basiccomponents/togglebutton.py` & `tkcomponents-3.0.0/tkcomponents/basiccomponents/togglebutton.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/component.py` & `tkcomponents-3.0.0/tkcomponents/component.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents/extensions/gridhelper.py` & `tkcomponents-3.0.0/tkcomponents/extensions/gridhelper.py`

 * *Files identical despite different names*

### Comparing `tkcomponents-2.1.2/tkcomponents.egg-info/PKG-INFO` & `tkcomponents-3.0.0/tkcomponents.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkcomponents
-Version: 2.1.2
+Version: 3.0.0
 Summary: An OOP framework for Tkinter, inspired by React
 Home-page: https://github.com/immijimmi/tkcomponents
-Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v2.1.2.tar.gz
+Download-URL: https://github.com/immijimmi/tkcomponents/archive/refs/tags/v3.0.0.tar.gz
 Author: immijimmi
 Author-email: immijimmi1@gmail.com
 License: MIT
 Keywords: ui,gui,graphical,user,interface
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `tkcomponents-2.1.2/tkcomponents.egg-info/SOURCES.txt` & `tkcomponents-3.0.0/tkcomponents.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 tkcomponents/__init__.py
 tkcomponents/component.py
 tkcomponents.egg-info/PKG-INFO
 tkcomponents.egg-info/SOURCES.txt
 tkcomponents.egg-info/dependency_links.txt
 tkcomponents.egg-info/requires.txt
 tkcomponents.egg-info/top_level.txt
-tkcomponents/abstractcomponents/__init__.py
-tkcomponents/abstractcomponents/timedframe.py
-tkcomponents/abstractcomponents/verticalscrollframe.py
 tkcomponents/basiccomponents/__init__.py
 tkcomponents/basiccomponents/alert.py
 tkcomponents/basiccomponents/buttonlistbox.py
 tkcomponents/basiccomponents/constants.py
 tkcomponents/basiccomponents/datestepper.py
 tkcomponents/basiccomponents/labelwrapper.py
 tkcomponents/basiccomponents/numberstepper.py
 tkcomponents/basiccomponents/numbersteppertable.py
 tkcomponents/basiccomponents/progressbar.py
 tkcomponents/basiccomponents/stringeditor.py
 tkcomponents/basiccomponents/textcarousel.py
+tkcomponents/basiccomponents/timedframe.py
 tkcomponents/basiccomponents/timercontrol.py
 tkcomponents/basiccomponents/togglebutton.py
+tkcomponents/basiccomponents/verticalscrollframe.py
 tkcomponents/basiccomponents/classes/dateticker.py
 tkcomponents/basiccomponents/classes/timer.py
 tkcomponents/extensions/__init__.py
+tkcomponents/extensions/draganddrop.py
 tkcomponents/extensions/gridhelper.py
```

