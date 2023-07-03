# Comparing `tmp/uitk-0.7.8.tar.gz` & `tmp/uitk-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uitk-0.7.8.tar", last modified: Mon Jul  3 15:10:49 2023, max compression
+gzip compressed data, was "uitk-0.7.9.tar", last modified: Mon Jul  3 15:11:22 2023, max compression
```

## Comparing `uitk-0.7.8.tar` & `uitk-0.7.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:49.543659 uitk-0.7.8/
--rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.7.8/COPYING.LESSER
--rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.7.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3691 2023-07-03 15:10:49.541384 uitk-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-03 15:10:49.543659 uitk-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-06-28 02:16:42.000000 uitk-0.7.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:49.494062 uitk-0.7.8/uitk/
--rw-rw-rw-   0        0        0     2937 2023-07-03 15:10:46.000000 uitk-0.7.8/uitk/__init__.py
--rw-rw-rw-   0        0        0    11209 2023-07-02 22:36:44.000000 uitk-0.7.8/uitk/events.py
--rw-rw-rw-   0        0        0    79273 2023-07-03 14:51:51.000000 uitk-0.7.8/uitk/switchboard.py
--rw-rw-rw-   0        0        0   100538 2023-07-01 11:42:38.000000 uitk-0.7.8/uitk/switchboard.py.bak
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:49.534385 uitk-0.7.8/uitk/widgets/
--rw-rw-rw-   0        0        0    19457 2023-07-02 22:38:42.000000 uitk-0.7.8/uitk/widgets/MainWindow.py
--rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.7.8/uitk/widgets/__init__.py
--rw-rw-rw-   0        0        0    15978 2023-06-29 12:22:22.000000 uitk-0.7.8/uitk/widgets/attributeWindow.py
--rw-rw-rw-   0        0        0     5597 2023-07-03 11:38:23.000000 uitk-0.7.8/uitk/widgets/checkBox.py
--rw-rw-rw-   0        0        0     7040 2023-07-03 11:08:37.000000 uitk-0.7.8/uitk/widgets/comboBox.py
--rw-rw-rw-   0        0        0     6954 2023-07-02 00:38:56.000000 uitk-0.7.8/uitk/widgets/draggableHeader.py
--rw-rw-rw-   0        0        0    22380 2023-07-03 00:41:20.000000 uitk-0.7.8/uitk/widgets/expandableList.py
--rw-rw-rw-   0        0        0     2494 2023-07-02 00:29:49.000000 uitk-0.7.8/uitk/widgets/label.py
--rw-rw-rw-   0        0        0     3234 2023-07-02 00:30:20.000000 uitk-0.7.8/uitk/widgets/lineEdit.py
--rw-rw-rw-   0        0        0    22049 2023-07-03 11:48:15.000000 uitk-0.7.8/uitk/widgets/menu.py
--rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.7.8/uitk/widgets/messageBox.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:49.540384 uitk-0.7.8/uitk/widgets/mixins/
--rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.7.8/uitk/widgets/mixins/__init__.py
--rw-rw-rw-   0        0        0    11901 2023-07-02 22:55:42.000000 uitk-0.7.8/uitk/widgets/mixins/attributes.py
--rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.7.8/uitk/widgets/mixins/convert.py
--rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.7.8/uitk/widgets/mixins/docking.py
--rw-rw-rw-   0        0        0    49547 2023-06-29 12:04:05.000000 uitk-0.7.8/uitk/widgets/mixins/style_sheet.py
--rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.7.8/uitk/widgets/mixins/tasks.py
--rw-rw-rw-   0        0        0    11111 2023-07-02 22:52:42.000000 uitk-0.7.8/uitk/widgets/mixins/text.py
--rw-rw-rw-   0        0        0     6046 2023-07-01 23:43:08.000000 uitk-0.7.8/uitk/widgets/optionBox.py
--rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.7.8/uitk/widgets/progressBar.py
--rw-rw-rw-   0        0        0     2113 2023-07-03 11:07:37.000000 uitk-0.7.8/uitk/widgets/pushButton.py
--rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.7.8/uitk/widgets/region.py
--rw-rw-rw-   0        0        0     3655 2023-07-02 00:31:26.000000 uitk-0.7.8/uitk/widgets/textEdit.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:10:49.517385 uitk-0.7.8/uitk.egg-info/
--rw-rw-rw-   0        0        0     3691 2023-07-03 15:10:49.000000 uitk-0.7.8/uitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.7.8/uitk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0      948 2023-07-03 15:10:49.000000 uitk-0.7.8/uitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.7.8/uitk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-07-03 15:10:49.000000 uitk-0.7.8/uitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-03 15:10:49.000000 uitk-0.7.8/uitk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.095646 uitk-0.7.9/
+-rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-0.7.9/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-03-28 23:38:26.000000 uitk-0.7.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3691 2023-07-03 15:11:22.095646 uitk-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-03 15:11:22.095646 uitk-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-06-28 02:16:42.000000 uitk-0.7.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.057646 uitk-0.7.9/uitk/
+-rw-rw-rw-   0        0        0     2937 2023-07-03 15:11:19.000000 uitk-0.7.9/uitk/__init__.py
+-rw-rw-rw-   0        0        0    11209 2023-07-02 22:36:44.000000 uitk-0.7.9/uitk/events.py
+-rw-rw-rw-   0        0        0    79273 2023-07-03 14:51:51.000000 uitk-0.7.9/uitk/switchboard.py
+-rw-rw-rw-   0        0        0   100538 2023-07-01 11:42:38.000000 uitk-0.7.9/uitk/switchboard.py.bak
+drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.086648 uitk-0.7.9/uitk/widgets/
+-rw-rw-rw-   0        0        0    19457 2023-07-02 22:38:42.000000 uitk-0.7.9/uitk/widgets/MainWindow.py
+-rw-rw-rw-   0        0        0     3204 2023-05-24 20:56:51.000000 uitk-0.7.9/uitk/widgets/__init__.py
+-rw-rw-rw-   0        0        0    15978 2023-06-29 12:22:22.000000 uitk-0.7.9/uitk/widgets/attributeWindow.py
+-rw-rw-rw-   0        0        0     5597 2023-07-03 11:38:23.000000 uitk-0.7.9/uitk/widgets/checkBox.py
+-rw-rw-rw-   0        0        0     7040 2023-07-03 11:08:37.000000 uitk-0.7.9/uitk/widgets/comboBox.py
+-rw-rw-rw-   0        0        0     6954 2023-07-02 00:38:56.000000 uitk-0.7.9/uitk/widgets/draggableHeader.py
+-rw-rw-rw-   0        0        0    22380 2023-07-03 00:41:20.000000 uitk-0.7.9/uitk/widgets/expandableList.py
+-rw-rw-rw-   0        0        0     2494 2023-07-02 00:29:49.000000 uitk-0.7.9/uitk/widgets/label.py
+-rw-rw-rw-   0        0        0     3234 2023-07-02 00:30:20.000000 uitk-0.7.9/uitk/widgets/lineEdit.py
+-rw-rw-rw-   0        0        0    22049 2023-07-03 11:48:15.000000 uitk-0.7.9/uitk/widgets/menu.py
+-rw-rw-rw-   0        0        0     8559 2023-06-23 14:22:44.000000 uitk-0.7.9/uitk/widgets/messageBox.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.094645 uitk-0.7.9/uitk/widgets/mixins/
+-rw-rw-rw-   0        0        0     3028 2023-05-12 17:13:16.000000 uitk-0.7.9/uitk/widgets/mixins/__init__.py
+-rw-rw-rw-   0        0        0    11901 2023-07-02 22:55:42.000000 uitk-0.7.9/uitk/widgets/mixins/attributes.py
+-rw-rw-rw-   0        0        0     4023 2023-05-12 17:25:02.000000 uitk-0.7.9/uitk/widgets/mixins/convert.py
+-rw-rw-rw-   0        0        0     9499 2023-05-20 02:33:14.000000 uitk-0.7.9/uitk/widgets/mixins/docking.py
+-rw-rw-rw-   0        0        0    49547 2023-06-29 12:04:05.000000 uitk-0.7.9/uitk/widgets/mixins/style_sheet.py
+-rw-rw-rw-   0        0        0     3409 2023-05-12 17:27:14.000000 uitk-0.7.9/uitk/widgets/mixins/tasks.py
+-rw-rw-rw-   0        0        0    11111 2023-07-02 22:52:42.000000 uitk-0.7.9/uitk/widgets/mixins/text.py
+-rw-rw-rw-   0        0        0     6046 2023-07-01 23:43:08.000000 uitk-0.7.9/uitk/widgets/optionBox.py
+-rw-rw-rw-   0        0        0     3278 2023-06-05 16:23:13.000000 uitk-0.7.9/uitk/widgets/progressBar.py
+-rw-rw-rw-   0        0        0     2113 2023-07-03 11:07:37.000000 uitk-0.7.9/uitk/widgets/pushButton.py
+-rw-rw-rw-   0        0        0     7907 2023-05-28 21:08:35.000000 uitk-0.7.9/uitk/widgets/region.py
+-rw-rw-rw-   0        0        0     3655 2023-07-02 00:31:26.000000 uitk-0.7.9/uitk/widgets/textEdit.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:11:22.070645 uitk-0.7.9/uitk.egg-info/
+-rw-rw-rw-   0        0        0     3691 2023-07-03 15:11:21.000000 uitk-0.7.9/uitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4282 2023-05-11 02:02:25.000000 uitk-0.7.9/uitk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0      948 2023-07-03 15:11:21.000000 uitk-0.7.9/uitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      767 2023-04-15 12:48:17.000000 uitk-0.7.9/uitk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-07-03 15:11:21.000000 uitk-0.7.9/uitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-03 15:11:21.000000 uitk-0.7.9/uitk.egg-info/top_level.txt
```

### Comparing `uitk-0.7.8/COPYING.LESSER` & `uitk-0.7.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/PKG-INFO` & `uitk-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.7.8
+Version: 0.7.9
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `uitk-0.7.8/setup.py` & `uitk-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/__init__.py` & `uitk-0.7.9/uitk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib
 import pkgutil
 import inspect
 from .switchboard import signals  # Make signals accessible at package root
 
 
 __package__ = "uitk"
-__version__ = '0.7.8'
+__version__ = '0.7.9'
 __path__ = [os.path.abspath(os.path.dirname(__file__))]
 
 
 # Define a dictionary to map class names to their respective modules
 CLASS_TO_MODULE = {}
 
 # Build the CLASS_TO_MODULE dictionary by iterating over all submodules of the package
```

### Comparing `uitk-0.7.8/uitk/events.py` & `uitk-0.7.9/uitk/events.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/switchboard.py` & `uitk-0.7.9/uitk/switchboard.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/switchboard.py.bak` & `uitk-0.7.9/uitk/switchboard.py.bak`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/MainWindow.py` & `uitk-0.7.9/uitk/widgets/MainWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/__init__.py` & `uitk-0.7.9/uitk/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/attributeWindow.py` & `uitk-0.7.9/uitk/widgets/attributeWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/checkBox.py` & `uitk-0.7.9/uitk/widgets/checkBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/comboBox.py` & `uitk-0.7.9/uitk/widgets/comboBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/draggableHeader.py` & `uitk-0.7.9/uitk/widgets/draggableHeader.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/expandableList.py` & `uitk-0.7.9/uitk/widgets/expandableList.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/label.py` & `uitk-0.7.9/uitk/widgets/label.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/lineEdit.py` & `uitk-0.7.9/uitk/widgets/lineEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/menu.py` & `uitk-0.7.9/uitk/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/messageBox.py` & `uitk-0.7.9/uitk/widgets/messageBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/mixins/__init__.py` & `uitk-0.7.9/uitk/widgets/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/mixins/attributes.py` & `uitk-0.7.9/uitk/widgets/mixins/attributes.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/mixins/convert.py` & `uitk-0.7.9/uitk/widgets/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/mixins/docking.py` & `uitk-0.7.9/uitk/widgets/mixins/docking.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/mixins/style_sheet.py` & `uitk-0.7.9/uitk/widgets/mixins/style_sheet.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/mixins/tasks.py` & `uitk-0.7.9/uitk/widgets/mixins/tasks.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/mixins/text.py` & `uitk-0.7.9/uitk/widgets/mixins/text.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/optionBox.py` & `uitk-0.7.9/uitk/widgets/optionBox.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/progressBar.py` & `uitk-0.7.9/uitk/widgets/progressBar.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/pushButton.py` & `uitk-0.7.9/uitk/widgets/pushButton.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/region.py` & `uitk-0.7.9/uitk/widgets/region.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk/widgets/textEdit.py` & `uitk-0.7.9/uitk/widgets/textEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk.egg-info/PKG-INFO` & `uitk-0.7.9/uitk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 0.7.8
+Version: 0.7.9
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `uitk-0.7.8/uitk.egg-info/PKG-INFO.bak` & `uitk-0.7.9/uitk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk.egg-info/SOURCES.txt` & `uitk-0.7.9/uitk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uitk-0.7.8/uitk.egg-info/SOURCES.txt.bak` & `uitk-0.7.9/uitk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

