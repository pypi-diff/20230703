# Comparing `tmp/linien-gui-0.8.0rc4.tar.gz` & `tmp/linien-gui-0.8.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-gui-0.8.0rc4.tar", last modified: Mon Jul  3 13:55:33 2023, max compression
+gzip compressed data, was "linien-gui-0.8.0rc5.tar", last modified: Mon Jul  3 14:11:56 2023, max compression
```

## Comparing `linien-gui-0.8.0rc4.tar` & `linien-gui-0.8.0rc5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:55:33.038818 linien-gui-0.8.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 13:55:33.038818 linien-gui-0.8.0rc4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:55:33.026818 linien-gui-0.8.0rc4/linien_gui/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)   410598 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:55:33.038818 linien-gui-0.8.0rc4/linien_gui/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/device_manager.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/general_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    26265 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/general_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/lock_status_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/locking_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/locking_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/logging_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/logging_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    42356 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/modulation_sweep_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/modulation_sweep_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/new_device_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/new_device_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/optimization_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/optimization_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/psd_plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/psd_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/psd_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/psd_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/right_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/spectroscopy_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/spectroscopy_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/spin_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/sweep_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/version_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/view_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/ui/view_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/linien_gui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:55:33.026818 linien-gui-0.8.0rc4/linien_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 13:55:33.000000 linien-gui-0.8.0rc4/linien_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-03 13:55:33.000000 linien-gui-0.8.0rc4/linien_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:55:33.000000 linien-gui-0.8.0rc4/linien_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 13:55:33.000000 linien-gui-0.8.0rc4/linien_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-03 13:55:33.000000 linien-gui-0.8.0rc4/linien_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 13:55:33.000000 linien-gui-0.8.0rc4/linien_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:55:33.038818 linien-gui-0.8.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-03 13:54:39.000000 linien-gui-0.8.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:56.160418 linien-gui-0.8.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 14:11:56.160418 linien-gui-0.8.0rc5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:56.152418 linien-gui-0.8.0rc5/linien_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   410598 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:56.160418 linien-gui-0.8.0rc5/linien_gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/device_manager.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/general_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26265 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/general_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/lock_status_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/locking_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/locking_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/logging_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/logging_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42356 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/modulation_sweep_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/modulation_sweep_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/new_device_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/new_device_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/optimization_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/optimization_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/psd_plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/psd_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/psd_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/psd_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/right_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/spectroscopy_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/spectroscopy_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/spin_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/sweep_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/view_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/ui/view_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/linien_gui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:11:56.152418 linien-gui-0.8.0rc5/linien_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 14:11:56.000000 linien-gui-0.8.0rc5/linien_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-03 14:11:56.000000 linien-gui-0.8.0rc5/linien_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:11:56.000000 linien-gui-0.8.0rc5/linien_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 14:11:56.000000 linien-gui-0.8.0rc5/linien_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-03 14:11:56.000000 linien-gui-0.8.0rc5/linien_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 14:11:56.000000 linien-gui-0.8.0rc5/linien_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:11:56.160418 linien-gui-0.8.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-03 14:10:51.000000 linien-gui-0.8.0rc5/setup.py
```

### Comparing `linien-gui-0.8.0rc4/PKG-INFO` & `linien-gui-0.8.0rc5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 0.8.0rc4
+Version: 0.8.0rc5
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-gui-0.8.0rc4/linien_gui/app.py` & `linien-gui-0.8.0rc5/linien_gui/app.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/config.py` & `linien-gui-0.8.0rc5/linien_gui/config.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/dialogs.py` & `linien-gui-0.8.0rc5/linien_gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/icon.ico` & `linien-gui-0.8.0rc5/linien_gui/icon.ico`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/threads.py` & `linien-gui-0.8.0rc5/linien_gui/threads.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/device_manager.py` & `linien-gui-0.8.0rc5/linien_gui/ui/device_manager.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/device_manager.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/device_manager.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/general_panel.py` & `linien-gui-0.8.0rc5/linien_gui/ui/general_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/general_panel.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/general_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/lock_status_panel.py` & `linien-gui-0.8.0rc5/linien_gui/ui/lock_status_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/locking_panel.py` & `linien-gui-0.8.0rc5/linien_gui/ui/locking_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/locking_panel.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/locking_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/logging_panel.py` & `linien-gui-0.8.0rc5/linien_gui/ui/logging_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/logging_panel.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/logging_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/main_window.py` & `linien-gui-0.8.0rc5/linien_gui/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/main_window.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/modulation_sweep_panel.py` & `linien-gui-0.8.0rc5/linien_gui/ui/modulation_sweep_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/modulation_sweep_panel.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/modulation_sweep_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/new_device_dialog.py` & `linien-gui-0.8.0rc5/linien_gui/ui/new_device_dialog.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/new_device_dialog.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/new_device_dialog.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/optimization_panel.py` & `linien-gui-0.8.0rc5/linien_gui/ui/optimization_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/optimization_panel.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/optimization_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/plot_widget.py` & `linien-gui-0.8.0rc5/linien_gui/ui/plot_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/psd_plot_widget.py` & `linien-gui-0.8.0rc5/linien_gui/ui/psd_plot_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/psd_table_widget.py` & `linien-gui-0.8.0rc5/linien_gui/ui/psd_table_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/psd_window.py` & `linien-gui-0.8.0rc5/linien_gui/ui/psd_window.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/psd_window.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/psd_window.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/right_panel.py` & `linien-gui-0.8.0rc5/linien_gui/ui/right_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/spectroscopy_panel.py` & `linien-gui-0.8.0rc5/linien_gui/ui/spectroscopy_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/spectroscopy_panel.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/spectroscopy_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/spin_box.py` & `linien-gui-0.8.0rc5/linien_gui/ui/spin_box.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/sweep_control.py` & `linien-gui-0.8.0rc5/linien_gui/ui/sweep_control.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/version_checker.py` & `linien-gui-0.8.0rc5/linien_gui/ui/version_checker.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/view_panel.py` & `linien-gui-0.8.0rc5/linien_gui/ui/view_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/ui/view_panel.ui` & `linien-gui-0.8.0rc5/linien_gui/ui/view_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/utils.py` & `linien-gui-0.8.0rc5/linien_gui/utils.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui/widgets.py` & `linien-gui-0.8.0rc5/linien_gui/widgets.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/linien_gui.egg-info/PKG-INFO` & `linien-gui-0.8.0rc5/linien_gui.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 0.8.0rc4
+Version: 0.8.0rc5
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-gui-0.8.0rc4/linien_gui.egg-info/SOURCES.txt` & `linien-gui-0.8.0rc5/linien_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc4/setup.py` & `linien-gui-0.8.0rc5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "0.8.0rc4"
+version = "0.8.0rc5"
 
 setup(
     name="linien-gui",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
```

