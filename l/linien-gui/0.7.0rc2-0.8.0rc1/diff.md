# Comparing `tmp/linien-gui-0.7.0rc2.tar.gz` & `tmp/linien-gui-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-gui-0.7.0rc2.tar", last modified: Tue Mar 21 15:48:10 2023, max compression
+gzip compressed data, was "linien-gui-0.8.0rc1.tar", last modified: Mon Jul  3 12:17:36 2023, max compression
```

## Comparing `linien-gui-0.7.0rc2.tar` & `linien-gui-0.8.0rc1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:48:10.173115 linien-gui-0.7.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-21 15:48:10.173115 linien-gui-0.7.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:48:10.169115 linien-gui-0.7.0rc2/linien_gui/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)   410598 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:48:10.173115 linien-gui-0.7.0rc2/linien_gui/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/device_manager.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/general_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    26265 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/general_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/lock_status_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/locking_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    39140 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/locking_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    41688 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/modulation_sweep_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/modulation_sweep_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/new_device_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/new_device_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/optimization_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/optimization_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)    30510 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/psd_plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/psd_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/psd_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/psd_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/right_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/spectroscopy_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/spectroscopy_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/spin_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/sweep_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/version_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/view_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/ui/view_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/linien_gui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:48:10.169115 linien-gui-0.7.0rc2/linien_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-21 15:48:10.000000 linien-gui-0.7.0rc2/linien_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-21 15:48:10.000000 linien-gui-0.7.0rc2/linien_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:48:10.000000 linien-gui-0.7.0rc2/linien_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-21 15:48:10.000000 linien-gui-0.7.0rc2/linien_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-21 15:48:10.000000 linien-gui-0.7.0rc2/linien_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-21 15:48:10.000000 linien-gui-0.7.0rc2/linien_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 15:48:10.173115 linien-gui-0.7.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-21 15:47:14.000000 linien-gui-0.7.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:36.193466 linien-gui-0.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 12:17:36.193466 linien-gui-0.8.0rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:36.189466 linien-gui-0.8.0rc1/linien_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   410598 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:36.193466 linien-gui-0.8.0rc1/linien_gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/device_manager.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/general_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26265 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/general_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/lock_status_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/locking_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/locking_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/logging_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/logging_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42356 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/modulation_sweep_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/modulation_sweep_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/new_device_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/new_device_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/optimization_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/optimization_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/psd_plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/psd_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/psd_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/psd_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/right_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/spectroscopy_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/spectroscopy_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/spin_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/sweep_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/view_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/ui/view_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/linien_gui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:17:36.189466 linien-gui-0.8.0rc1/linien_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 12:17:36.000000 linien-gui-0.8.0rc1/linien_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-03 12:17:36.000000 linien-gui-0.8.0rc1/linien_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:17:36.000000 linien-gui-0.8.0rc1/linien_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 12:17:36.000000 linien-gui-0.8.0rc1/linien_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-03 12:17:36.000000 linien-gui-0.8.0rc1/linien_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 12:17:36.000000 linien-gui-0.8.0rc1/linien_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 12:17:36.193466 linien-gui-0.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-03 12:16:37.000000 linien-gui-0.8.0rc1/setup.py
```

### Comparing `linien-gui-0.7.0rc2/PKG-INFO` & `linien-gui-0.8.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 0.7.0rc2
+Version: 0.8.0rc1
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/app.py` & `linien-gui-0.8.0rc1/linien_gui/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,92 +16,72 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import signal
 import sys
 from traceback import print_exc
 
 import click
-import linien_gui
-from linien_gui.ui.device_manager import DeviceManager
-from linien_gui.ui.main_window import MainWindow
-from linien_gui.ui.psd_window import PSDWindow
-from linien_gui.ui.version_checker import VersionCheckerThread
-from linien_gui.utils import set_window_icon
-from linien_gui.widgets import UI_PATH, CustomWidget
+from linien_client.connection import LinienClient
 from PyQt5 import QtWidgets
+from PyQt5.QtCore import pyqtSignal
 from pyqtgraph.Qt import QtCore
 
+from . import __version__
+from .config import load_settings
+from .ui.device_manager import DeviceManager
+from .ui.main_window import MainWindow
+from .ui.psd_window import PSDWindow
+from .ui.version_checker import VersionCheckerThread
+from .widgets import UI_PATH
+
 sys.path += [str(UI_PATH)]
 
 
-class QTApp(QtCore.QObject):
-    def __init__(self):
-        self.app = QtWidgets.QApplication(sys.argv)
+class LinienApp(QtWidgets.QApplication):
+    connection_established = pyqtSignal()
 
-        self.main_window = MainWindow()
-        self.main_window.app = self
-        set_window_icon(self.main_window)
+    def __init__(self, *args, **kwargs):
+        super(LinienApp, self).__init__(*args, **kwargs)
 
-        self.device_manager = DeviceManager()
-        self.device_manager.app = self
-        self.device_manager.show()
+        self.settings = load_settings()
 
+        self.main_window = MainWindow()
+        self.device_manager = DeviceManager()
         self.psd_window = PSDWindow()
-        self.psd_window.app = self
-
-        self.app.aboutToQuit.connect(lambda: self.app.quit())
+        self.device_manager.show()
 
-        super().__init__()
+        self.aboutToQuit.connect(self.quit)
 
-    def client_connected(self, client):
+    def client_connected(self, client: LinienClient):
         self.device_manager.hide()
         self.main_window.show(client.host, client.name)
 
         self.client = client
         self.control = client.control
         self.parameters = client.parameters
 
-        for instance in CustomWidget.instances:
-            try:
-                instance.on_connection_established()
-            except Exception:
-                print(
-                    (
-                        "The error below happend when calling connection_established "
-                        "of a widget. This may happen if the widget was recently "
-                        "destroyed."
-                    )
-                )
-                print_exc()
+        self.connection_established.emit()
 
-        self.call_listeners()
+        self.periodically_check_for_changed_parameters()
 
         self.check_for_new_version()
 
-    def call_listeners(self):
+    def periodically_check_for_changed_parameters(self):
         if hasattr(self, "client") and self.client and self.client.connected:
             try:
-                self.parameters.call_listeners()
+                self.parameters.check_for_changed_parameters()
             except AttributeError:
-                print("call_listeners() failed")
+                print("check_for_changed_parameters() failed")
                 print_exc()
 
-            QtCore.QTimer.singleShot(50, self.call_listeners)
-
-    def get_widget(self, name, window=None):
-        """Queries a widget by name."""
-        window = window or self.main_window
-        return window.findChild(QtCore.QObject, name)
-
-    def close(self):
-        self.app.quit()
+            QtCore.QTimer.singleShot(50, self.periodically_check_for_changed_parameters)
 
     def shutdown(self):
-        self.client.control.shutdown()
-        self.close()
+        self.client.control.exposed_shutdown()
+        self.quit()
 
     def open_psd_window(self):
         # first hiding it, then showing it brings it to foregroud if it is in background
         self.psd_window.hide()
         self.psd_window.show()
 
     def open_device_manager(self):
@@ -125,18 +105,18 @@
             self.main_window.show_new_version_available()
         else:
             print("No new version available")
             QtCore.QTimer.singleShot(1000 * 60 * 60, self.check_for_new_version)
 
 
 @click.command()
-@click.version_option(linien_gui.__version__)
+@click.version_option(__version__)
 def run_application():
-    gui = QTApp()
+    app = LinienApp(sys.argv)
 
     # catch ctrl-c and shutdown
     signal.signal(signal.SIGINT, signal.SIG_DFL)
-    sys.exit(gui.app.exec_())
+    sys.exit(app.exec_())
 
 
 if __name__ == "__main__":
     run_application()
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/config.py` & `linien-gui-0.8.0rc1/linien_gui/ui/new_device_dialog.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,83 +11,48 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-import os
-import pickle
-from enum import Enum
+import random
+import string
 
-import appdirs
-import rpyc
-
-# don't plot more often than once per `DEFAULT_PLOT_RATE_LIMIT` seconds
-DEFAULT_PLOT_RATE_LIMIT = 0.1
-
-
-class Color(Enum):
-    SPECTRUM1 = 0
-    SPECTRUM2 = 1
-    SPECTRUM_COMBINED = 2
-    CONTROL_SIGNAL = 0
-    CONTROL_SIGNAL_HISTORY = 1
-    SLOW_HISTORY = 3
-    MONITOR_SIGNAL_HISTORY = 4
-
-
-def get_data_folder():
-    folder_name = appdirs.user_data_dir("linien")
-
-    if not os.path.exists(folder_name):
-        os.makedirs(folder_name)
-
-    return folder_name
-
-
-def get_devices_filename():
-    return os.path.join(get_data_folder(), "devices")
-
-
-def save_device_data(devices):
-    with open(get_devices_filename(), "wb") as f:
-        pickle.dump(devices, f)
-
-
-def load_device_data():
-    try:
-        with open(get_devices_filename(), "rb") as f:
-            devices = pickle.load(f)
-    except (FileNotFoundError, pickle.UnpicklingError, EOFError):
-        devices = []
-
-    return devices
-
-
-def save_parameter(device_key, param, value, delete=False):
-    devices = load_device_data()
-    device = [d for d in devices if d["key"] == device_key][0]
-    device.setdefault("params", {})
-
-    if not delete:
-        # FIXME: This is the only part where rpyc is used in linien-gui. Remove it if
-        # possible.
-        # rpyc obtain is for ensuring that we don't try to save a netref here
-        try:
-            device["params"][param] = rpyc.classic.obtain(value)
-        except Exception:
-            print("unable to obtain and save parameter", param)
-    else:
-        try:
-            del device["params"][param]
-        except KeyError:
-            pass
-
-    save_device_data(devices)
-
-
-def get_saved_parameters(device_key):
-    devices = load_device_data()
-    device = [d for d in devices if d["key"] == device_key][0]
-    device.setdefault("params", {})
-    return device["params"]
+from linien_common.config import DEFAULT_SERVER_PORT
+from linien_gui.config import load_device_data, save_device_data
+from linien_gui.widgets import UI_PATH
+from PyQt5 import QtWidgets, uic
+
+
+class NewDeviceDialog(QtWidgets.QDialog):
+    def __init__(self, initial_device=None):
+        super(NewDeviceDialog, self).__init__()
+        uic.loadUi(UI_PATH / "new_device_dialog.ui", self)
+
+        if initial_device is not None:
+            self.deviceName.setText(initial_device["name"])
+            self.host.setText(initial_device["host"])
+            self.username.setText(initial_device["username"])
+            self.password.setText(initial_device["password"])
+            self.port.setValue(initial_device.get("port", DEFAULT_SERVER_PORT))
+            self.explain_host.setVisible(False)
+            self.key = initial_device["key"]
+        else:
+            self.key = "".join(random.choice(string.ascii_lowercase) for i in range(10))
+
+    def add_new_device(self):
+        device = {
+            "key": self.key,
+            "name": self.deviceName.text(),
+            "host": self.host.text(),
+            "username": self.username.text(),
+            "password": self.password.text(),
+            "port": self.port.value(),
+            "params": {},
+        }
+
+        old_devices = [
+            device for device in load_device_data() if device["key"] != self.key
+        ]
+        devices = old_devices + [device]
+        save_device_data(devices)
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/dialogs.py` & `linien-gui-0.8.0rc1/linien_gui/dialogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,39 +11,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-from time import sleep
 from typing import Callable
 
-from linien_gui.threads import RemoteServerInstallationThread
-from PyQt5.QtCore import QThread, pyqtSignal
+from PyQt5.QtCore import pyqtSignal
 from PyQt5.QtWidgets import (
     QDialog,
     QListWidget,
     QMessageBox,
     QPushButton,
     QVBoxLayout,
     QWidget,
 )
 from pyqtgraph import QtCore
 
+from .threads import RemoteServerInstallationThread
+
 
 class SSHCommandOutputWidget(QListWidget):
     command_finished = pyqtSignal()
     enable_button = pyqtSignal()
 
     def __init__(self, parent: QWidget):
-        super().__init__(parent)
+        super(SSHCommandOutputWidget, self).__init__(parent)
         self.setSelectionMode(self.NoSelection)
 
-    def run(self, thread: QThread):
+    def run(self, thread):
         self.thread = thread
         self.thread.out_stream.new_item.connect(self.on_new_item_in_out_stream)
         self.thread.finished.connect(self.on_thread_finished)
         self.thread.start()
 
     def on_new_item_in_out_stream(self, line: str):
         self.addItem(line.rstrip())
@@ -82,15 +82,15 @@
     return window
 
 
 class LoadingDialog(QMessageBox):
     aborted = pyqtSignal()
 
     def __init__(self, parent: QWidget, host: str):
-        super().__init__(parent)
+        super(LoadingDialog, self).__init__(parent)
 
         self.setIcon(QMessageBox.Information)
         self.setText(f"Connecting to {host}")
         self.setWindowTitle("Connecting")
         self.setModal(True)
         self.setWindowModality(QtCore.Qt.WindowModal)
         self.setStandardButtons(QMessageBox.NoButton)
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/icon.ico` & `linien-gui-0.8.0rc1/linien_gui/icon.ico`

 * *Files identical despite different names*

### Comparing `linien-gui-0.7.0rc2/linien_gui/threads.py` & `linien-gui-0.8.0rc1/linien_gui/threads.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 from linien_client.exceptions import (
     GeneralConnectionErrorException,
     InvalidServerVersionException,
     RPYCAuthenticationException,
     ServerNotInstalledException,
 )
 from linien_common.config import DEFAULT_SERVER_PORT
-from linien_gui.config import get_saved_parameters, save_parameter
 from PyQt5.QtCore import QObject, QThread, pyqtSignal
 
+from .config import get_saved_parameters, save_parameter
+
 
 class RemoteOutStream(QObject):
     new_item = pyqtSignal(str)
 
     def write(self, item):
         self.new_item.emit(item)
 
@@ -41,33 +42,33 @@
         pass
 
     def flush(self):
         pass
 
 
 class RemoteServerInstallationThread(QThread):
-    def __init__(self, device):
+    def __init__(self, device: dict):
         """A thread that installs the linien server on a remote machine."""
-        super().__init__()
+        super(RemoteServerInstallationThread, self).__init__()
         self.device = device
 
     out_stream = RemoteOutStream()
 
     def run(self):
         install_remote_server(
             host=self.device["host"],
             user=self.device["username"],
             password=self.device["password"],
             out_stream=self.out_stream,
         )
 
 
 class ConnectionThread(QThread):
-    def __init__(self, device):
-        super().__init__()
+    def __init__(self, device: dict):
+        super(ConnectionThread, self).__init__()
         self.device = device
 
     client_connected = pyqtSignal(object)
     server_not_installed_exception_raised = pyqtSignal()
     invalid_server_version_exception_raised = pyqtSignal(str, str)
     authentication_exception_raised = pyqtSignal()
     general_connection_exception_raised = pyqtSignal()
@@ -97,15 +98,15 @@
                 self.ask_for_parameter_restore.emit()
             else:
                 # if parameters don't differ, we can start monitoring remote parameter
                 # changes and write them to disk. We don't do this if parameters differ
                 # because we don't want to override our local settings with the remote
                 # one --> we wait until user has answered whether local parameters or
                 # remote ones should be used.
-                self.continuously_write_parameters_to_disk()
+                self.write_restorable_parameters_to_disk_on_change()
 
         except ServerNotInstalledException:
             self.server_not_installed_exception_raised.emit()
 
         except InvalidServerVersionException as e:
             self.invalid_server_version_exception_raised.emit(
                 e.remote_version, e.client_version
@@ -124,27 +125,26 @@
     def on_connection_lost(self):
         self.connection_lost.emit()
 
     def answer_whether_to_restore_parameters(self, should_restore):
         if should_restore:
             self.restore_parameters(dry_run=False)
 
-        self.continuously_write_parameters_to_disk()
+        self.write_restorable_parameters_to_disk_on_change()
 
     def restore_parameters(self, dry_run=False):
         """
         Reads settings for a server that were cached locally. Sends them to the server.
         If `dry_run` is...
 
             * `True`, this function returns a boolean indicating whether the
               local parameters differ from the ones on the server
             * `False`, the local parameters are uploaded to the server
         """
-        device_key = self.device["key"]
-        params = get_saved_parameters(device_key)
+        params = get_saved_parameters(self.device["key"])
         print("restoring parameters")
 
         differences = False
 
         for k, v in params.items():
             if hasattr(self.client.parameters, k):
                 param = getattr(self.client.parameters, k)
@@ -155,28 +155,27 @@
                         break
                     else:
                         param.value = v
             else:
                 # This may happen if the settings were written with a different version
                 # of linien.
                 print(f"Unable to restore parameter {k}. Delete the cached value.")
-                save_parameter(device_key, k, None, delete=True)
+                save_parameter(self.device["key"], k, None, delete=True)
 
         if not dry_run:
             self.client.control.write_registers()
 
         return differences
 
-    def continuously_write_parameters_to_disk(self):
+    def write_restorable_parameters_to_disk_on_change(self):
         """
         Listens for changes of some parameters and permanently saves their values on the
         client's disk. This data can be used to restore the status later, if the client
         tries to connect to the server but it doesn't run anymore.
         """
-        params = self.client.parameters.remote.exposed_get_restorable_parameters()
-
-        for param in params:
+        for parameter_name, parameter in self.client.parameters:
+            if parameter.restorable:
 
-            def on_change(value, param=param):
-                save_parameter(self.device["key"], param, value)
+                def on_change(value, parameter_name: str = parameter_name) -> None:
+                    save_parameter(self.device["key"], parameter_name, value)
 
-            getattr(self.client.parameters, param).on_change(on_change)
+                parameter.add_callback(on_change)
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/device_manager.py` & `linien-gui-0.8.0rc1/linien_gui/ui/device_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,38 +23,37 @@
     ask_for_parameter_restore_dialog,
     error_dialog,
     question_dialog,
     show_installation_progress_widget,
 )
 from linien_gui.threads import ConnectionThread
 from linien_gui.ui.new_device_dialog import NewDeviceDialog
-from linien_gui.utils import set_window_icon
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtCore, QtWidgets
+from linien_gui.utils import get_linien_app_instance, set_window_icon
+from linien_gui.widgets import UI_PATH
+from PyQt5 import QtCore, QtWidgets, uic
 
 
-class DeviceManager(QtWidgets.QMainWindow, CustomWidget):
+class DeviceManager(QtWidgets.QMainWindow):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.load_ui("device_manager.ui")
+        super(DeviceManager, self).__init__(*args, **kwargs)
+        uic.loadUi(UI_PATH / "device_manager.ui", self)
         self.setWindowTitle(f"Linien spectroscopy lock v{linien_gui.__version__}")
         set_window_icon(self)
-
-    def ready(self):
-        self.load_device_data(autoload=True)
+        self.app = get_linien_app_instance()
+        QtCore.QTimer.singleShot(100, lambda: self.load_device_data(autoload=True))
 
     def keyPressEvent(self, event):
         key = event.key()
 
         if key in (QtCore.Qt.Key_Enter, QtCore.Qt.Key_Return):
             self.connect()
 
     def load_device_data(self, autoload=False):
         devices = load_device_data()
-        lst = self.ids.deviceList
+        lst = self.deviceList
         lst.clear()
 
         for device in devices:
             lst.addItem("{} ({})".format(device["name"], device["host"]))
 
         if autoload and len(devices) == 1:
             self.connect_to_device(devices[0])
@@ -63,15 +62,15 @@
         devices = load_device_data()
 
         if not devices:
             return
         else:
             self.connect_to_device(devices[self.get_list_index()])
 
-    def connect_to_device(self, device):
+    def connect_to_device(self, device: dict):
         loading_dialog = LoadingDialog(self, device["host"])
         loading_dialog.show()
 
         aborted = {}
 
         self.connection_thread = ConnectionThread(device)
 
@@ -159,15 +158,15 @@
             should_restore = ask_for_parameter_restore_dialog(
                 self, question, "Restore parameters?"
             )
             self.connection_thread.answer_whether_to_restore_parameters(should_restore)
 
         def handle_connection_lost():
             error_dialog(self, "Lost connection to the server!")
-            self.app.close()
+            self.app.quit()
 
         # Connect slots to signals -----------------------------------------------------
         self.connection_thread.client_connected.connect(on_client_connected)
 
         self.connection_thread.server_not_installed_exception_raised.connect(
             handle_server_not_installed
         )
@@ -236,18 +235,18 @@
         if new_index < 0 or new_index > len(devices) - 1:
             return
 
         device = devices.pop(current_index)
         devices = devices[:new_index] + [device] + devices[new_index:]
         save_device_data(devices)
         self.load_device_data()
-        self.ids.deviceList.setCurrentRow(new_index)
+        self.deviceList.setCurrentRow(new_index)
 
     def get_list_index(self):
-        return self.ids.deviceList.currentIndex().row()
+        return self.deviceList.currentIndex().row()
 
     def remove_device(self):
         devices = load_device_data()
 
         if not devices:
             return
 
@@ -263,14 +262,14 @@
         if idx >= 0:
             devices = load_device_data()
 
             if devices:
                 disable_buttons = False
 
         for btn in [
-            self.ids.connectButton,
-            self.ids.removeButton,
-            self.ids.editButton,
-            self.ids.moveUpButton,
-            self.ids.moveDownButton,
+            self.connectButton,
+            self.removeButton,
+            self.editButton,
+            self.moveUpButton,
+            self.moveDownButton,
         ]:
             btn.setEnabled(not disable_buttons)
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/device_manager.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/device_manager.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/general_panel.py` & `linien-gui-0.8.0rc1/linien_gui/ui/general_panel.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 from linien_common.common import (
     ANALOG_OUT0,
     ANALOG_OUT_V,
     FAST_OUT1,
     FAST_OUT2,
     convert_channel_mixing_value,
 )
-from linien_gui.utils import param2ui
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import get_linien_app_instance, param2ui
+from linien_gui.widgets import UI_PATH
+from PyQt5 import QtWidgets, uic
 
 
-class GeneralPanel(QtWidgets.QWidget, CustomWidget):
+class GeneralPanel(QtWidgets.QWidget):
     def __init__(self, *args, **kwargs):
         super(GeneralPanel, self).__init__(*args, **kwargs)
-        self.load_ui("general_panel.ui")
+        uic.loadUi(UI_PATH / "general_panel.ui", self)
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
 
         self.channelMixingSlider.valueChanged.connect(self.on_channel_mixing_changed)
         self.fastModeCheckBox.stateChanged.connect(self.on_fast_mode_changed)
         self.dualChannelCheckBox.stateChanged.connect(self.on_dual_channel_changed)
         self.modulationChannelComboBox.currentIndexChanged.connect(
             self.on_mod_channel_changed
         )
@@ -55,17 +57,15 @@
         self.polarityComboBoxFastOut2.currentIndexChanged.connect(
             self.on_polarity_fast_out2_changed
         )
         self.polarityComboBoxAnalogOut0.currentIndexChanged.connect(
             self.on_polarity_analog_out0_changed
         )
 
-        for idx in range(4):
-            if idx == 0:
-                continue
+        for idx in range(1, 4):
             element = getattr(self, f"analogOutComboBox{idx}")
             element.setKeyboardTracking(False)
             element.valueChanged.connect(
                 lambda _, idx=idx: self.on_analog_out_changed(idx)
             )
 
     def on_connection_established(self):
@@ -101,23 +101,21 @@
         param2ui(self.parameters.sweep_channel, self.sweepChannelComboBox)
         param2ui(self.parameters.slow_control_channel, self.slowControlComboBox)
 
         param2ui(self.parameters.polarity_fast_out1, self.polarityComboBoxFastOut1)
         param2ui(self.parameters.polarity_fast_out2, self.polarityComboBoxFastOut2)
         param2ui(self.parameters.polarity_analog_out0, self.polarityComboBoxAnalogOut0)
 
-        self.parameters.control_channel.on_change(self.show_polarity_settings)
-        self.parameters.sweep_channel.on_change(self.show_polarity_settings)
-        self.parameters.mod_channel.on_change(self.show_polarity_settings)
-        self.parameters.slow_control_channel.on_change(self.show_polarity_settings)
-        self.parameters.pid_on_slow_enabled.on_change(self.show_polarity_settings)
-
-        for idx in range(4):
-            if idx == 0:
-                continue
+        self.parameters.control_channel.add_callback(self.show_polarity_settings)
+        self.parameters.sweep_channel.add_callback(self.show_polarity_settings)
+        self.parameters.mod_channel.add_callback(self.show_polarity_settings)
+        self.parameters.slow_control_channel.add_callback(self.show_polarity_settings)
+        self.parameters.pid_on_slow_enabled.add_callback(self.show_polarity_settings)
+
+        for idx in range(1, 4):
             param2ui(
                 getattr(self.parameters, f"analog_out_{idx}"),
                 getattr(self, f"analogOutComboBox{idx}"),
                 process_value=lambda v: ANALOG_OUT_V * v,
             )
 
         def on_fast_mode_changed(fast_mode_enabled):
@@ -125,15 +123,15 @@
             widgets_to_disable = (
                 self.output_ports_group,
                 self.input_ports_group,
             )
             for widget in widgets_to_disable:
                 widget.setEnabled(not fast_mode_enabled)
 
-        self.parameters.fast_mode.on_change(on_fast_mode_changed)
+        self.parameters.fast_mode.add_callback(on_fast_mode_changed)
 
     def on_analog_out_changed(self, idx):
         getattr(self.parameters, f"analog_out_{idx}").value = int(
             getattr(self, f"analogOutComboBox{idx}").value() / ANALOG_OUT_V
         )
         self.control.write_registers()
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/general_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/general_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/lock_status_panel.py` & `linien-gui-0.8.0rc1/linien_gui/ui/lock_status_panel.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,28 +12,31 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-from linien_gui.utils import param2ui
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import get_linien_app_instance, param2ui
+from PyQt5 import QtCore, QtWidgets
 
 
-class LockStatusPanel(QtWidgets.QWidget, CustomWidget):
+class LockStatusPanel(QtWidgets.QWidget):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super(LockStatusPanel, self).__init__(*args, **kwargs)
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
+        QtCore.QTimer.singleShot(100, self.ready)
 
     def ready(self):
-        self.ids.stop_lock.clicked.connect(self.stop_lock)
-        self.ids.control_signal_history_length.setKeyboardTracking(False)
-        self.ids.control_signal_history_length.valueChanged.connect(
-            self.control_signal_history_length_changed
+        self.parent = self.parent()
+        self.parent.stopLockPushButton.clicked.connect(self.on_stop_lock)
+        self.parent.controlSignalHistoryLengthSpinBox.setKeyboardTracking(False)
+        self.parent.controlSignalHistoryLengthSpinBox.valueChanged.connect(
+            self.on_control_signal_history_length_changed
         )
 
     def on_connection_established(self):
         self.parameters = self.app.parameters
         self.control = self.app.control
 
         def update_status(_):
@@ -53,53 +56,51 @@
             if task:
                 watching = self.parameters.autolock_watching.value
             else:
                 running = False
                 watching = False
 
             def set_text(text):
-                self.ids.lock_status.setText(text)
+                self.parent.lock_status.setText(text)
 
             if not running and locked:
                 set_text("Locked!")
             if running and watching:
                 set_text("Locked! Watching continuously...")
             if running and not watching and not locked and preparing:
                 if not retrying:
-                    set_text(
-                        "Autolock is running... Analyzing data (%d %%)" % percentage
-                    )
+                    set_text(f"Autolock is running... Analyzing data ({percentage} %%)")
                 else:
                     set_text("Trying again to lock...")
 
         for param in (
             self.parameters.lock,
             self.parameters.task,
             self.parameters.autolock_running,
             self.parameters.autolock_preparing,
             self.parameters.autolock_watching,
             self.parameters.autolock_failed,
             self.parameters.autolock_locked,
             self.parameters.autolock_retrying,
             self.parameters.autolock_percentage,
         ):
-            param.on_change(update_status)
+            param.add_callback(update_status)
 
         param2ui(
             self.parameters.control_signal_history_length,
-            self.ids.control_signal_history_length,
+            self.parent.controlSignalHistoryLengthSpinBox,
         )
 
-    def stop_lock(self):
+    def on_stop_lock(self):
         self.parameters.fetch_additional_signals.value = True
 
         if self.parameters.task.value is not None:
             # this may be autolock or psd acquisition
             self.parameters.task.value.stop()
             self.parameters.task.value = None
 
         self.control.exposed_start_sweep()
 
-    def control_signal_history_length_changed(self):
+    def on_control_signal_history_length_changed(self):
         self.parameters.control_signal_history_length.value = (
-            self.ids.control_signal_history_length.value()
+            self.parent.controlSignalHistoryLengthSpinBox.value()
         )
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/locking_panel.py` & `linien-gui-0.8.0rc1/linien_gui/ui/locking_panel.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,166 +13,146 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from linien_common.common import FAST_AUTOLOCK
-from linien_gui.utils import param2ui
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import get_linien_app_instance, param2ui
+from linien_gui.widgets import UI_PATH
+from PyQt5 import QtWidgets, uic
 
 
-class LockingPanel(QtWidgets.QWidget, CustomWidget):
+class LockingPanel(QtWidgets.QWidget):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.load_ui("locking_panel.ui")
+        super(LockingPanel, self).__init__(*args, **kwargs)
+        uic.loadUi(UI_PATH / "locking_panel.ui", self)
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
+
+        self.kpSpinBox.valueChanged.connect(self.kp_changed)
+        self.kiSpinBox.valueChanged.connect(self.ki_changed)
+        self.kdSpinBox.valueChanged.connect(self.kd_changed)
+        self.lock_control_container.currentChanged.connect(self.lock_mode_changed)
 
-    def ready(self):
-        self.ids.kp.valueChanged.connect(self.kp_changed)
-        self.ids.ki.valueChanged.connect(self.ki_changed)
-        self.ids.kd.valueChanged.connect(self.kd_changed)
-        # self.ids.checkLockCheckbox.stateChanged.connect(self.check_lock_changed)
-        # self.ids.watchLockCheckbox.stateChanged.connect(self.watch_lock_changed)
-        # self.ids.watch_lock_threshold.valueChanged.connect(
-        #    self.watch_lock_threshold_changed
-        # )
-        self.ids.lock_control_container.currentChanged.connect(self.lock_mode_changed)
+        self.selectLineToLock.clicked.connect(self.start_autolock_selection)
+        self.abortLineSelection.clicked.connect(self.stop_autolock_selection)
 
-        self.ids.selectLineToLock.clicked.connect(self.start_autolock_selection)
-        self.ids.abortLineSelection.clicked.connect(self.stop_autolock_selection)
+        self.manualLockButton.clicked.connect(self.start_manual_lock)
+        self.autoOffsetCheckbox.stateChanged.connect(self.auto_offset_changed)
 
-        self.ids.manualLockButton.clicked.connect(self.start_manual_lock)
-        self.ids.autoOffsetCheckbox.stateChanged.connect(self.auto_offset_changed)
-
-        self.ids.pid_on_slow_strength.setKeyboardTracking(False)
-        self.ids.pid_on_slow_strength.valueChanged.connect(
+        self.pid_on_slow_strength.setKeyboardTracking(False)
+        self.pid_on_slow_strength.valueChanged.connect(
             self.pid_on_slow_strength_changed
         )
 
-        self.ids.reset_lock_failed_state.clicked.connect(self.reset_lock_failed)
+        self.reset_lock_failed_state.clicked.connect(self.reset_lock_failed)
 
-        self.ids.autolock_mode_preference.currentIndexChanged.connect(
+        self.autolock_mode_preference.currentIndexChanged.connect(
             self.autolock_mode_preference_changed
         )
 
     def on_connection_established(self):
         self.parameters = self.app.parameters
         self.control = self.app.control
 
-        param2ui(self.parameters.p, self.ids.kp)
-        param2ui(self.parameters.i, self.ids.ki)
-        param2ui(self.parameters.d, self.ids.kd)
-
-        # param2ui(params.check_lock, self.ids.checkLockCheckbox)
-        # param2ui(params.watch_lock, self.ids.watchLockCheckbox)
-        # param2ui(
-        #    params.watch_lock_threshold,
-        #    self.ids.watch_lock_threshold,
-        #    lambda v: v * 100,
-        # )
-        param2ui(self.parameters.autolock_determine_offset, self.ids.autoOffsetCheckbox)
+        param2ui(self.parameters.p, self.kpSpinBox)
+        param2ui(self.parameters.i, self.kiSpinBox)
+        param2ui(self.parameters.d, self.kdSpinBox)
+
+        param2ui(self.parameters.autolock_determine_offset, self.autoOffsetCheckbox)
         param2ui(
             self.parameters.automatic_mode,
-            self.ids.lock_control_container,
+            self.lock_control_container,
             lambda value: 0 if value else 1,
         )
-        param2ui(self.parameters.pid_on_slow_strength, self.ids.pid_on_slow_strength)
+        param2ui(self.parameters.pid_on_slow_strength, self.pid_on_slow_strength)
 
         def slow_pid_visibility(*args):
-            self.ids.slow_pid_group.setVisible(
-                self.parameters.pid_on_slow_enabled.value
-            )
+            self.slow_pid_group.setVisible(self.parameters.pid_on_slow_enabled.value)
 
-        self.parameters.pid_on_slow_enabled.on_change(slow_pid_visibility)
+        self.parameters.pid_on_slow_enabled.add_callback(slow_pid_visibility)
 
         def lock_status_changed(_):
             locked = self.parameters.lock.value
             task = self.parameters.task.value
             al_failed = self.parameters.autolock_failed.value
             task_running = (task is not None) and (not al_failed)
 
             if locked or task_running or al_failed:
-                self.ids.lock_control_container.hide()
+                self.lock_control_container.hide()
             else:
-                self.ids.lock_control_container.show()
+                self.lock_control_container.show()
 
-            self.ids.lock_failed.setVisible(al_failed)
+            self.lock_failed.setVisible(al_failed)
 
         for param in (
             self.parameters.lock,
             self.parameters.autolock_preparing,
             self.parameters.autolock_watching,
             self.parameters.autolock_failed,
             self.parameters.autolock_locked,
         ):
-            param.on_change(lock_status_changed)
+            param.add_callback(lock_status_changed)
 
-        param2ui(self.parameters.target_slope_rising, self.ids.button_slope_rising)
+        param2ui(self.parameters.target_slope_rising, self.button_slope_rising)
         param2ui(
             self.parameters.target_slope_rising,
-            self.ids.button_slope_falling,
+            self.button_slope_falling,
             lambda value: not value,
         )
 
         def autolock_selection_status_changed(value):
-            self.ids.auto_mode_activated.setVisible(value)
-            self.ids.auto_mode_not_activated.setVisible(not value)
+            self.auto_mode_activated.setVisible(value)
+            self.auto_mode_not_activated.setVisible(not value)
 
-        self.parameters.autolock_selection.on_change(autolock_selection_status_changed)
+        self.parameters.autolock_selection.add_callback(
+            autolock_selection_status_changed
+        )
 
         param2ui(
-            self.parameters.autolock_mode_preference, self.ids.autolock_mode_preference
+            self.parameters.autolock_mode_preference, self.autolock_mode_preference
         )
 
     def kp_changed(self):
-        self.parameters.p.value = self.ids.kp.value()
+        self.parameters.p.value = self.kpSpinBox.value()
         self.control.write_registers()
 
     def ki_changed(self):
-        self.parameters.i.value = self.ids.ki.value()
+        self.parameters.i.value = self.kiSpinBox.value()
         self.control.write_registers()
 
     def kd_changed(self):
-        self.parameters.d.value = self.ids.kd.value()
+        self.parameters.d.value = self.kdSpinBox.value()
         self.control.write_registers()
 
     def lock_mode_changed(self, idx):
         self.parameters.automatic_mode.value = idx == 0
 
     def autolock_mode_preference_changed(self, idx):
         self.parameters.autolock_mode_preference.value = idx
 
     def start_manual_lock(self):
-        self.parameters.target_slope_rising.value = (
-            self.ids.button_slope_rising.isChecked()
-        )
+        self.parameters.target_slope_rising.value = self.button_slope_rising.isChecked()
         self.parameters.fetch_additional_signals.value = False
         self.parameters.autolock_mode.value = FAST_AUTOLOCK
         self.parameters.autolock_target_position.value = 0
         self.control.write_registers()
         self.control.start_lock()
 
     def auto_offset_changed(self):
         self.parameters.autolock_determine_offset.value = int(
-            self.ids.autoOffsetCheckbox.checkState()
+            self.autoOffsetCheckbox.checkState()
         )
 
     def pid_on_slow_strength_changed(self):
-        self.parameters.pid_on_slow_strength.value = (
-            self.ids.pid_on_slow_strength.value()
-        )
+        self.parameters.pid_on_slow_strength.value = self.pid_on_slow_strength.value()
         self.control.write_registers()
 
     def start_autolock_selection(self):
         self.parameters.autolock_selection.value = True
 
     def stop_autolock_selection(self):
         self.parameters.autolock_selection.value = False
 
-    """def watch_lock_threshold_changed(self):
-        self.parameters.watch_lock_threshold.value = (
-            self.ids.watch_lock_threshold.value() / 100.0
-        )"""
-
     def reset_lock_failed(self):
         self.parameters.autolock_failed.value = False
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/locking_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/locking_panel.ui`

 * *Files 1% similar despite different names*

#### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/locking_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/locking_panel.ui`

```diff
@@ -75,15 +75,15 @@
                       </property>
                       <property name="alignment">
                         <set>Qt::AlignCenter</set>
                       </property>
                     </widget>
                   </item>
                   <item>
-                    <widget class="CustomSpinBox" name="kp">
+                    <widget class="CustomSpinBox" name="kpSpinBox">
                       <property name="keyboardTracking">
                         <bool>false</bool>
                       </property>
                       <property name="minimum">
                         <number>0</number>
                       </property>
                       <property name="maximum">
@@ -153,15 +153,15 @@
                       </property>
                       <property name="alignment">
                         <set>Qt::AlignCenter</set>
                       </property>
                     </widget>
                   </item>
                   <item>
-                    <widget class="CustomSpinBox" name="ki">
+                    <widget class="CustomSpinBox" name="kiSpinBox">
                       <property name="keyboardTracking">
                         <bool>false</bool>
                       </property>
                       <property name="minimum">
                         <number>0</number>
                       </property>
                       <property name="maximum">
@@ -234,15 +234,15 @@
                       </property>
                       <property name="alignment">
                         <set>Qt::AlignCenter</set>
                       </property>
                     </widget>
                   </item>
                   <item>
-                    <widget class="CustomSpinBox" name="kd">
+                    <widget class="CustomSpinBox" name="kdSpinBox">
                       <property name="sizePolicy">
                         <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
                           <horstretch>0</horstretch>
                           <verstretch>0</verstretch>
                         </sizepolicy>
                       </property>
                       <property name="keyboardTracking">
@@ -691,15 +691,15 @@
                 </property>
                 <property name="wordWrap">
                   <bool>true</bool>
                 </property>
               </widget>
             </item>
             <item>
-              <widget class="QPushButton" name="stop_lock">
+              <widget class="QPushButton" name="stopLockPushButton">
                 <property name="palette">
                   <palette>
                     <active>
                       <colorrole role="WindowText">
                         <brush brushstyle="SolidPattern">
                           <color alpha="255">
                             <red>0</red>
@@ -1128,15 +1128,15 @@
                   </sizepolicy>
                 </property>
                 <property name="title">
                   <string>Control signal history length</string>
                 </property>
                 <layout class="QHBoxLayout" name="horizontalLayout_9">
                   <item>
-                    <widget class="CustomSpinBox" name="control_signal_history_length">
+                    <widget class="CustomSpinBox" name="controlSignalHistoryLengthSpinBox">
                       <property name="minimum">
                         <number>10</number>
                       </property>
                       <property name="maximum">
                         <number>100000</number>
                       </property>
                       <property name="singleStep">
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/main_window.py` & `linien-gui-0.8.0rc1/linien_gui/ui/main_window.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,82 +20,153 @@
 import pickle
 from math import log
 from time import time
 
 import linien_gui
 import numpy as np
 from linien_common.common import check_plot_data
-from linien_common.config import N_COLORS
-from linien_gui.config import Color
+from linien_gui.config import N_COLORS, Color
 from linien_gui.ui.plot_widget import INVALID_POWER
-from linien_gui.utils import color_to_hex
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import color_to_hex, get_linien_app_instance, set_window_icon
+from linien_gui.widgets import UI_PATH
+from PyQt5 import QtWidgets, uic
 
 ZOOM_STEP = 0.9
 MAX_ZOOM = 50
 MIN_ZOOM = 0
 
 
 def sweep_amplitude_to_zoom_step(amplitude):
     return round(log(amplitude, ZOOM_STEP))
 
 
-class MainWindow(QtWidgets.QMainWindow, CustomWidget):
+class MainWindow(QtWidgets.QMainWindow):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.load_ui("main_window.ui")
+        super(MainWindow, self).__init__(*args, **kwargs)
+        uic.loadUi(UI_PATH / "main_window.ui", self)
+        set_window_icon(self)
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
 
         self.reset_std_history()
 
-    def show(self, host, name):
-        self.setWindowTitle(
-            "Linien spectroscopy lock %s: %s (%s)"
-            % (linien_gui.__version__, name, host)
-        )
-        super().show()
-
-    def closeEvent(self, *args, **kwargs):
-        self.app.close_all_secondary_windows()
-        super().closeEvent(*args, **kwargs)
-
-    def ready(self):
         # handle keyboard events
         self.setFocus()
 
-        self.ids.export_parameters_button.clicked.connect(
+        self.export_parameters_button.clicked.connect(
             self.export_parameters_select_file
         )
-        self.ids.import_parameters_button.clicked.connect(self.import_parameters)
+        self.import_parameters_button.clicked.connect(self.import_parameters)
 
         def display_power(power, element):
             if power == INVALID_POWER:
                 element.hide()
             else:
                 element.show()
-                text = "%.2f" % power
-                element.setText(text)
+                element.setText(f"{power:.2f}")
 
         def display_power_channel_1(power):
-            el = self.ids.power_channel_1
+            el = self.power_channel_1
             display_power(power, el)
 
         def display_power_channel_2(power):
-            el = self.ids.power_channel_2
+            el = self.power_channel_2
             display_power(power, el)
 
-        self.ids.graphicsView.signal_power1.connect(display_power_channel_1)
-        self.ids.graphicsView.signal_power2.connect(display_power_channel_2)
-        self.ids.graphicsView.keyPressed.connect(self.handle_key_press)
+        self.graphicsView.signal_power1.connect(display_power_channel_1)
+        self.graphicsView.signal_power2.connect(display_power_channel_2)
+        self.graphicsView.keyPressed.connect(self.handle_key_press)
 
         # by default we hide it and just show when a new version is available
-        self.ids.new_version_available_label.hide()
+        self.newVersionAvailableLabel.hide()
+
+    def on_connection_established(self):
+        self.control = self.app.control
+        self.parameters = self.app.parameters
+
+        self.parameters.lock.add_callback(self.change_sweep_control_visibility)
+        self.parameters.autolock_running.add_callback(
+            self.change_sweep_control_visibility
+        )
+        self.parameters.optimization_running.add_callback(
+            self.change_sweep_control_visibility
+        )
+
+        self.parameters.to_plot.add_callback(self.update_std)
+
+        self.parameters.pid_on_slow_enabled.add_callback(
+            lambda v: self.legend_slow_signal_history.setVisible(v)
+        )
+        self.parameters.dual_channel.add_callback(
+            lambda v: self.legend_monitor_signal_history.setVisible(not v)
+        )
+
+        self.settings_toolbox.setCurrentIndex(0)
+
+        self.parameters.lock.add_callback(lambda *args: self.reset_std_history())
+
+        for color_idx in range(N_COLORS):
+            getattr(self.app.settings, f"plot_color_{color_idx}").add_callback(
+                self.update_legend_color
+            )
+
+        self.parameters.dual_channel.add_callback(self.update_legend_text)
+
+    def change_sweep_control_visibility(self, *args):
+        al_running = self.parameters.autolock_running.value
+        optimization = self.parameters.optimization_running.value
+        locked = self.parameters.lock.value
+
+        self.sweepControlWidget.setVisible(
+            not al_running and not locked and not optimization
+        )
+        self.top_lock_panel.setVisible(locked)
+        self.statusbar_unlocked.setVisible(
+            not al_running and not locked and not optimization
+        )
+
+    def update_legend_color(self, *args):
+        def set_color(el, color: Color):
+            return el.setStyleSheet(
+                "color: "
+                + color_to_hex(
+                    getattr(self.app.settings, f"plot_color_{color.value}").value
+                )
+            )
+
+        set_color(self.legend_spectrum_1, Color.SPECTRUM1)
+        set_color(self.legend_spectrum_2, Color.SPECTRUM2)
+        set_color(self.legend_spectrum_combined, Color.SPECTRUM_COMBINED)
+        set_color(self.legend_error_signal, Color.SPECTRUM_COMBINED)
+        set_color(self.legend_control_signal, Color.CONTROL_SIGNAL)
+        set_color(self.legend_control_signal_history, Color.CONTROL_SIGNAL_HISTORY)
+        set_color(self.legend_slow_signal_history, Color.SLOW_HISTORY)
+        set_color(self.legend_monitor_signal_history, Color.MONITOR_SIGNAL_HISTORY)
+
+    def update_legend_text(self, dual_channel):
+        self.legend_spectrum_1.setText(
+            "error signal" if not dual_channel else "error signal 1"
+        )
+        self.legend_spectrum_2.setText(
+            "monitor" if not dual_channel else "error signal 2"
+        )
+        self.legend_spectrum_combined.setVisible(dual_channel)
+
+    def show(self, host, name):
+        self.setWindowTitle(
+            f"Linien spectroscopy lock {linien_gui.__version__}: {name} ({host})"
+        )
+        super().show()
+
+    def closeEvent(self, *args, **kwargs):
+        self.app.close_all_secondary_windows()
+        super().closeEvent(*args, **kwargs)
 
     def show_new_version_available(self):
-        self.ids.new_version_available_label.show()
+        self.newVersionAvailableLabel.show()
 
     def handle_key_press(self, key):
         print("key pressed", key)
 
     def export_parameters_select_file(self):
         options = QtWidgets.QFileDialog.Options()
         # options |= QtWidgets.QFileDialog.DontUseNativeDialog
@@ -112,122 +183,46 @@
                 fn = fn + default_ext
 
             with open(fn, "w") as f:
                 json.dump(
                     {
                         "linien-version": linien_gui.__version__,
                         "time": time(),
-                        "parameters": dict(
-                            (k, getattr(self.parameters, k).value)
-                            for k in self.parameters.remote.exposed_get_restorable_parameters()  # noqa: E501
-                        ),
+                        "parameters": {
+                            name: param.value
+                            for name, param in self.parameters
+                            if param.restorable
+                        },
                     },
                     f,
                 )
 
     def import_parameters(self):
         options = QtWidgets.QFileDialog.Options()
-        # options |= QtWidgets.QFileDialog.DontUseNativeDialog
-        default_ext = ".json"
         fn, _ = QtWidgets.QFileDialog.getOpenFileName(
             self,
             "QFileDialog.getSaveFileName()",
             "",
-            "JSON (*%s)" % default_ext,
+            "JSON (*.json)",
             options=options,
         )
         if fn:
             with open(fn, "r") as f:
                 data = json.load(f)
 
-            assert "linien-version" in data, "invalid parameter file"
+            if "linien-version" not in data:
+                raise Exception("invalid parameter file")
 
-            restorable = self.parameters.remote.exposed_get_restorable_parameters()
-            for k, v in data["parameters"].items():
-                if k not in restorable:
-                    print("ignore key", k)
-                    continue
-
-                print("restoring", k)
-                getattr(self.parameters, k).value = v
+            for name, value in data["parameters"].items():
+                param = getattr(self.parameters, name)
+                if param.restorable:
+                    param.value = value
 
             self.control.write_registers()
 
-    def on_connection_established(self):
-        self.control = self.app.control
-        self.parameters = self.app.parameters
-
-        def change_sweep_control_visibility(*args):
-            al_running = self.parameters.autolock_running.value
-            optimization = self.parameters.optimization_running.value
-            locked = self.parameters.lock.value
-
-            self.get_widget("sweep_control").setVisible(
-                not al_running and not locked and not optimization
-            )
-            self.get_widget("top_lock_panel").setVisible(locked)
-            self.get_widget("statusbar_unlocked").setVisible(
-                not al_running and not locked and not optimization
-            )
-
-        self.parameters.lock.on_change(change_sweep_control_visibility)
-        self.parameters.autolock_running.on_change(change_sweep_control_visibility)
-        self.parameters.optimization_running.on_change(change_sweep_control_visibility)
-
-        self.parameters.to_plot.on_change(self.update_std)
-
-        self.parameters.pid_on_slow_enabled.on_change(
-            lambda v: self.ids.legend_slow_signal_history.setVisible(v)
-        )
-        self.parameters.dual_channel.on_change(
-            lambda v: self.ids.legend_monitor_signal_history.setVisible(not v)
-        )
-
-        self.ids.settings_toolbox.setCurrentIndex(0)
-
-        self.parameters.lock.on_change(lambda *args: self.reset_std_history())
-
-        def update_legend_color(*args):
-            def set_color(el, color: Color):
-                return el.setStyleSheet(
-                    "color: "
-                    + color_to_hex(
-                        getattr(self.parameters, f"plot_color_{color.value}").value
-                    )
-                )
-
-            set_color(self.ids.legend_spectrum_1, Color.SPECTRUM1)
-            set_color(self.ids.legend_spectrum_2, Color.SPECTRUM2)
-            set_color(self.ids.legend_spectrum_combined, Color.SPECTRUM_COMBINED)
-            set_color(self.ids.legend_error_signal, Color.SPECTRUM_COMBINED)
-            set_color(self.ids.legend_control_signal, Color.CONTROL_SIGNAL)
-            set_color(
-                self.ids.legend_control_signal_history, Color.CONTROL_SIGNAL_HISTORY
-            )
-            set_color(self.ids.legend_slow_signal_history, Color.SLOW_HISTORY)
-            set_color(
-                self.ids.legend_monitor_signal_history, Color.MONITOR_SIGNAL_HISTORY
-            )
-
-        for color_idx in range(N_COLORS):
-            getattr(self.parameters, "plot_color_%d" % color_idx).on_change(
-                update_legend_color
-            )
-
-        def update_legend_text(dual_channel):
-            self.ids.legend_spectrum_1.setText(
-                "error signal" if not dual_channel else "error signal 1"
-            )
-            self.ids.legend_spectrum_2.setText(
-                "monitor" if not dual_channel else "error signal 2"
-            )
-            self.ids.legend_spectrum_combined.setVisible(dual_channel)
-
-        self.parameters.dual_channel.on_change(update_legend_text)
-
     def update_std(self, to_plot, max_std_history_length=10):
         if self.parameters.lock.value and to_plot:
             to_plot = pickle.loads(to_plot)
             if to_plot and check_plot_data(True, to_plot):
                 error_signal = to_plot.get("error_signal")
                 control_signal = to_plot.get("control_signal")
 
@@ -238,15 +233,13 @@
                     -max_std_history_length:
                 ]
                 self.control_std_history = self.control_std_history[
                     -max_std_history_length:
                 ]
 
                 if error_signal is not None and control_signal is not None:
-                    self.ids.error_std.setText("%.2f" % np.mean(self.error_std_history))
-                    self.ids.control_std.setText(
-                        "%.2f" % np.mean(self.control_std_history)
-                    )
+                    self.error_std.setText("%.2f" % np.mean(self.error_std_history))
+                    self.control_std.setText(f"{np.mean(self.control_std_history):.2f}")
 
     def reset_std_history(self):
         self.error_std_history = []
         self.control_std_history = []
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/main_window.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/main_window.ui`

 * *Files 1% similar despite different names*

#### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/main_window.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/main_window.ui`

```diff
@@ -29,31 +29,31 @@
                 <verstretch>0</verstretch>
               </sizepolicy>
             </property>
             <layout class="QHBoxLayout" name="horizontalLayout_8">
               <item>
                 <layout class="QVBoxLayout" name="verticalLayout_17">
                   <item>
-                    <widget class="SweepControlWidget" name="sweep_control" native="true">
+                    <widget class="SweepControlWidget" name="sweepControlWidget" native="true">
                       <layout class="QHBoxLayout" name="horizontalLayout_3">
                         <item>
-                          <widget class="QLabel" name="label_9">
+                          <widget class="QLabel" name="sweepLabel">
                             <property name="font">
                               <font>
                                 <weight>75</weight>
                                 <bold>true</bold>
                               </font>
                             </property>
                             <property name="text">
                               <string>Sweep:</string>
                             </property>
                           </widget>
                         </item>
                         <item>
-                          <widget class="QPushButton" name="sweep_start_stop_button">
+                          <widget class="QPushButton" name="sweepStartStopPushButton">
                             <property name="toolTip">
                               <string>&lt;!DOCTYPE HTML PUBLIC &quot;-//W3C//DTD HTML 4.0//EN&quot; &quot;http://www.w3.org/TR/REC-html40/strict.dtd&quot;&gt;
 &lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
 p, li { white-space: pre-wrap; }
 &lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'MS Shell Dlg 2'; font-size:8pt; font-weight:400; font-style:normal;&quot;&gt;
 &lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Start and pause the output of the sweep at the sweep center position.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                             </property>
@@ -75,15 +75,15 @@
                                 <width>40</width>
                                 <height>20</height>
                               </size>
                             </property>
                           </spacer>
                         </item>
                         <item>
-                          <widget class="SweepSlider" name="sweep_slider">
+                          <widget class="SweepSlider" name="sweepSlider">
                             <property name="minimumSize">
                               <size>
                                 <width>350</width>
                                 <height>0</height>
                               </size>
                             </property>
                             <property name="maximum">
@@ -104,28 +104,28 @@
                                 <width>40</width>
                                 <height>20</height>
                               </size>
                             </property>
                           </spacer>
                         </item>
                         <item>
-                          <widget class="QLabel" name="label_2">
+                          <widget class="QLabel" name="sweepCenterLabel">
                             <property name="font">
                               <font>
                                 <weight>75</weight>
                                 <bold>true</bold>
                               </font>
                             </property>
                             <property name="text">
                               <string>Center:</string>
                             </property>
                           </widget>
                         </item>
                         <item>
-                          <widget class="CustomDoubleSpinBox" name="sweep_center">
+                          <widget class="CustomDoubleSpinBox" name="sweepCenterSpinBox">
                             <property name="minimumSize">
                               <size>
                                 <width>65</width>
                                 <height>0</height>
                               </size>
                             </property>
                             <property name="toolTip">
@@ -155,28 +155,28 @@
                             </property>
                             <property name="value">
                               <double>0.000000000000000</double>
                             </property>
                           </widget>
                         </item>
                         <item>
-                          <widget class="QLabel" name="label_3">
+                          <widget class="QLabel" name="sweepAmplitudeLabel">
                             <property name="font">
                               <font>
                                 <weight>75</weight>
                                 <bold>true</bold>
                               </font>
                             </property>
                             <property name="text">
                               <string>Amplitude:</string>
                             </property>
                           </widget>
                         </item>
                         <item>
-                          <widget class="CustomDoubleSpinBox" name="sweep_amplitude">
+                          <widget class="CustomDoubleSpinBox" name="sweepAmplitudeSpinBox">
                             <property name="minimumSize">
                               <size>
                                 <width>65</width>
                                 <height>0</height>
                               </size>
                             </property>
                             <property name="toolTip">
@@ -522,15 +522,15 @@
               <size>
                 <width>350</width>
                 <height>0</height>
               </size>
             </property>
             <layout class="QVBoxLayout" name="verticalLayout_11">
               <item>
-                <widget class="QLabel" name="new_version_available_label">
+                <widget class="QLabel" name="newVersionAvailableLabel">
                   <property name="text">
                     <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p align=&quot;center&quot;&gt;&lt;span style=&quot; font-size:14pt; font-weight:600; color:#3ebd46;&quot;&gt;New Linien version available:&lt;/span&gt;&lt;/p&gt;&lt;p align=&quot;center&quot;&gt;&lt;a href=&quot;https://github.com/linien-org/linien/&quot;&gt;&lt;span style=&quot; font-size:14pt; font-weight:600; text-decoration: underline; color:#1a5fb4;&quot;&gt;Download&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                   </property>
                   <property name="margin">
                     <number>10</number>
                   </property>
                   <property name="openExternalLinks">
@@ -1040,26 +1040,26 @@
                   <property name="minimumSize">
                     <size>
                       <width>250</width>
                       <height>0</height>
                     </size>
                   </property>
                   <property name="currentIndex">
-                    <number>2</number>
+                    <number>3</number>
                   </property>
                   <widget class="QWidget" name="generalPanel">
                     <property name="enabled">
                       <bool>true</bool>
                     </property>
                     <property name="geometry">
                       <rect>
                         <x>0</x>
                         <y>0</y>
-                        <width>98</width>
-                        <height>28</height>
+                        <width>332</width>
+                        <height>400</height>
                       </rect>
                     </property>
                     <attribute name="label">
                       <string>General</string>
                     </attribute>
                     <layout class="QVBoxLayout" name="verticalLayout_15">
                       <item>
@@ -1068,16 +1068,16 @@
                     </layout>
                   </widget>
                   <widget class="QWidget" name="modSpectroscopyPanel">
                     <property name="geometry">
                       <rect>
                         <x>0</x>
                         <y>0</y>
-                        <width>98</width>
-                        <height>28</height>
+                        <width>332</width>
+                        <height>400</height>
                       </rect>
                     </property>
                     <attribute name="label">
                       <string>Modulation, Sweep &amp;&amp; Spectroscopy</string>
                     </attribute>
                     <layout class="QVBoxLayout" name="verticalLayout_3">
                       <item>
@@ -1087,33 +1087,48 @@
                   </widget>
                   <widget class="QWidget" name="optimizationPanel">
                     <property name="geometry">
                       <rect>
                         <x>0</x>
                         <y>0</y>
                         <width>332</width>
-                        <height>427</height>
+                        <height>400</height>
                       </rect>
                     </property>
                     <attribute name="label">
                       <string>Optimization</string>
                     </attribute>
                     <layout class="QVBoxLayout" name="verticalLayout_10">
                       <item>
                         <widget class="OptimizationPanel" name="widget_6" native="true"/>
                       </item>
                     </layout>
                   </widget>
+                  <widget class="QWidget" name="logging">
+                    <attribute name="label">
+                      <string>Logging</string>
+                    </attribute>
+                    <widget class="LoggingPanel" name="widget_7" native="true">
+                      <property name="geometry">
+                        <rect>
+                          <x>0</x>
+                          <y>0</y>
+                          <width>321</width>
+                          <height>401</height>
+                        </rect>
+                      </property>
+                    </widget>
+                  </widget>
                   <widget class="QWidget" name="viewPanel">
                     <property name="geometry">
                       <rect>
                         <x>0</x>
                         <y>0</y>
-                        <width>98</width>
-                        <height>28</height>
+                        <width>332</width>
+                        <height>400</height>
                       </rect>
                     </property>
                     <property name="sizePolicy">
                       <sizepolicy hsizetype="Minimum" vsizetype="Preferred">
                         <horstretch>0</horstretch>
                         <verstretch>0</verstretch>
                       </sizepolicy>
@@ -1128,16 +1143,16 @@
                     </layout>
                   </widget>
                   <widget class="QWidget" name="lockingPanel">
                     <property name="geometry">
                       <rect>
                         <x>0</x>
                         <y>0</y>
-                        <width>98</width>
-                        <height>28</height>
+                        <width>332</width>
+                        <height>400</height>
                       </rect>
                     </property>
                     <property name="sizePolicy">
                       <sizepolicy hsizetype="Minimum" vsizetype="Preferred">
                         <horstretch>0</horstretch>
                         <verstretch>0</verstretch>
                       </sizepolicy>
@@ -1225,11 +1240,17 @@
       <container>1</container>
     </customwidget>
     <customwidget>
       <class>CustomDoubleSpinBox</class>
       <extends>QDoubleSpinBox</extends>
       <header location="global">spin_box.h</header>
     </customwidget>
+    <customwidget>
+      <class>LoggingPanel</class>
+      <extends>QWidget</extends>
+      <header>logging_panel.h</header>
+      <container>1</container>
+    </customwidget>
   </customwidgets>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/modulation_sweep_panel.py` & `linien-gui-0.8.0rc1/linien_gui/ui/modulation_sweep_panel.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,91 +13,92 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from linien_common.common import MHz, Vpp
-from linien_gui.utils import param2ui
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import get_linien_app_instance, param2ui
+from linien_gui.widgets import UI_PATH
+from PyQt5 import QtWidgets, uic
 
 
-class ModulationAndSweepPanel(QtWidgets.QWidget, CustomWidget):
+class ModulationAndSweepPanel(QtWidgets.QWidget):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.load_ui("modulation_sweep_panel.ui")
+        super(ModulationAndSweepPanel, self).__init__(*args, **kwargs)
+        uic.loadUi(UI_PATH / "modulation_sweep_panel.ui", self)
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
 
-    def ready(self):
-        self.ids.modulation_frequency.setKeyboardTracking(False)
-        self.ids.modulation_frequency.valueChanged.connect(
+        self.modulationFrequencySpinBox.setKeyboardTracking(False)
+        self.modulationFrequencySpinBox.valueChanged.connect(
             self.change_modulation_frequency
         )
-        self.ids.modulation_amplitude.setKeyboardTracking(False)
-        self.ids.modulation_amplitude.valueChanged.connect(
+        self.modulationAmplitudeSpinBox.setKeyboardTracking(False)
+        self.modulationAmplitudeSpinBox.valueChanged.connect(
             self.change_modulation_amplitude
         )
-        self.ids.sweep_speed.currentIndexChanged.connect(self.change_sweep_speed)
+        self.sweepSpeedComboBox.currentIndexChanged.connect(self.change_sweep_speed)
 
-        self.ids.spectroscopyTabs.setCurrentIndex(0)
+        self.spectroscopyTabs.setCurrentIndex(0)
 
     def on_connection_established(self):
         self.parameters = self.app.parameters
         self.control = self.app.control
 
         param2ui(
             self.parameters.modulation_frequency,
-            self.ids.modulation_frequency,
+            self.modulationFrequencySpinBox,
             lambda value: value / MHz,
         )
         param2ui(
             self.parameters.modulation_amplitude,
-            self.ids.modulation_amplitude,
+            self.modulationAmplitudeSpinBox,
             lambda value: value / Vpp,
         )
-        param2ui(self.parameters.sweep_speed, self.ids.sweep_speed)
+        param2ui(self.parameters.sweep_speed, self.sweepSpeedComboBox)
 
-        self.parameters.dual_channel.on_change(self.dual_channel_changed)
+        self.parameters.dual_channel.add_callback(self.dual_channel_changed)
 
         def fast_mode_changed(fast_mode_enabled):
             """Disables controls that are irrelevant if fast mode is enabled"""
             widgets_to_disable = (
-                self.ids.modulation_frequency_group,
-                self.ids.modulation_amplitude_group,
-                self.ids.spectroscopyTabs,
+                self.modulation_frequency_group,
+                self.modulation_amplitude_group,
+                self.spectroscopyTabs,
             )
             for widget in widgets_to_disable:
                 widget.setEnabled(not fast_mode_enabled)
 
-        self.parameters.fast_mode.on_change(fast_mode_changed)
+        self.parameters.fast_mode.add_callback(fast_mode_changed)
 
         def fast_mode_changed(fast_mode_enabled):
             """Disables controls that are irrelevant if fast mode is enabled"""
             widgets_to_disable = (
-                self.ids.modulation_frequency_group,
-                self.ids.modulation_amplitude_group,
-                self.ids.spectroscopyTabs,
+                self.modulation_frequency_group,
+                self.modulation_amplitude_group,
+                self.spectroscopyTabs,
             )
             for widget in widgets_to_disable:
                 widget.setEnabled(not fast_mode_enabled)
 
-        self.parameters.fast_mode.on_change(fast_mode_changed)
+        self.parameters.fast_mode.add_callback(fast_mode_changed)
 
     def change_modulation_frequency(self):
         self.parameters.modulation_frequency.value = (
-            self.ids.modulation_frequency.value() * MHz
+            self.modulationFrequencySpinBox.value() * MHz
         )
         self.control.write_registers()
 
     def change_modulation_amplitude(self):
         self.parameters.modulation_amplitude.value = (
-            self.ids.modulation_amplitude.value() * Vpp
+            self.modulationAmplitudeSpinBox.value() * Vpp
         )
         self.control.write_registers()
 
     def change_sweep_speed(self, decimation):
         self.parameters.sweep_speed.value = decimation
         self.control.write_registers()
 
     def dual_channel_changed(self, value):
-        self.ids.spectroscopyBPanel.setEnabled(value)
-        self.ids.spectroscopyBPanelDisabled.setVisible(not value)
+        self.spectroscopyBPanel.setEnabled(value)
+        self.spectroscopyBPanelDisabled.setVisible(not value)
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/modulation_sweep_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/modulation_sweep_panel.ui`

 * *Files 1% similar despite different names*

#### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/modulation_sweep_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/modulation_sweep_panel.ui`

```diff
@@ -22,15 +22,15 @@
           <property name="title">
             <string>Modulation frequency</string>
           </property>
           <layout class="QVBoxLayout" name="verticalLayout_5">
             <item>
               <layout class="QHBoxLayout" name="horizontalLayout_6">
                 <item>
-                  <widget class="CustomDoubleSpinBoxNoSign" name="modulation_frequency">
+                  <widget class="CustomDoubleSpinBoxNoSign" name="modulationFrequencySpinBox">
                     <property name="decimals">
                       <number>5</number>
                     </property>
                   </widget>
                 </item>
                 <item>
                   <widget class="QLabel" name="label_5">
@@ -59,15 +59,15 @@
           <property name="title">
             <string>Modulation amplitude</string>
           </property>
           <layout class="QVBoxLayout" name="verticalLayout_2">
             <item>
               <layout class="QHBoxLayout" name="horizontalLayout_2">
                 <item>
-                  <widget class="CustomDoubleSpinBoxNoSign" name="modulation_amplitude">
+                  <widget class="CustomDoubleSpinBoxNoSign" name="modulationAmplitudeSpinBox">
                     <property name="decimals">
                       <number>3</number>
                     </property>
                     <property name="maximum">
                       <double>2.000000000000000</double>
                     </property>
                     <property name="singleStep">
@@ -92,15 +92,15 @@
           <property name="title">
             <string>Sweep speed</string>
           </property>
           <layout class="QVBoxLayout" name="verticalLayout_4">
             <item>
               <layout class="QHBoxLayout" name="horizontalLayout_5">
                 <item>
-                  <widget class="QComboBox" name="sweep_speed">
+                  <widget class="QComboBox" name="sweepSpeedComboBox">
                     <property name="sizePolicy">
                       <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
                         <horstretch>0</horstretch>
                         <verstretch>0</verstretch>
                       </sizepolicy>
                     </property>
                     <item>
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/new_device_dialog.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/new_device_dialog.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/optimization_panel.py` & `linien-gui-0.8.0rc1/linien_gui/ui/optimization_panel.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,98 +13,95 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from linien_common.common import MHz, Vpp
-from linien_gui.utils import param2ui
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import get_linien_app_instance, param2ui
+from linien_gui.widgets import UI_PATH
+from PyQt5 import QtWidgets, uic
 
 
-class OptimizationPanel(QtWidgets.QWidget, CustomWidget):
+class OptimizationPanel(QtWidgets.QWidget):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.load_ui("optimization_panel.ui")
-
-    def ready(self):
-        self.ids.start_optimization_btn.clicked.connect(self.start_optimization)
-        self.ids.optimization_use_new_parameters.clicked.connect(
-            self.use_new_parameters
-        )
-        self.ids.optimization_abort.clicked.connect(self.abort)
-        self.ids.abortOptimizationLineSelection.clicked.connect(self.abort_selection)
-        self.ids.abortOptimizationPreparing.clicked.connect(self.abort_preparation)
-        self.ids.optimization_channel_selector.currentIndexChanged.connect(
+        super(OptimizationPanel, self).__init__(*args, **kwargs)
+        uic.loadUi(UI_PATH / "optimization_panel.ui", self)
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
+
+        self.startOptimizationPushButton.clicked.connect(self.start_optimization)
+        self.useOptimizedParametersPushButton.clicked.connect(self.use_new_parameters)
+        self.optimization_abort.clicked.connect(self.abort)
+        self.abortOptimizationLineSelection.clicked.connect(self.abort_selection)
+        self.abortOptimizationPreparing.clicked.connect(self.abort_preparation)
+        self.optimizationChannelComboBox.currentIndexChanged.connect(
             self.channel_changed
         )
-        self.ids.optimization_reset_failed_state.clicked.connect(
-            self.reset_failed_state
-        )
+        self.optimization_reset_failed_state.clicked.connect(self.reset_failed_state)
 
         for param_name in (
             "optimization_mod_freq_min",
             "optimization_mod_freq_max",
             "optimization_mod_amp_min",
             "optimization_mod_amp_max",
         ):
-            element = getattr(self.ids, param_name)
+            element = getattr(self, param_name)
             element.setKeyboardTracking(False)
 
             def write_parameter(*args, param_name=param_name, element=element):
                 getattr(self.parameters, param_name).value = element.value()
 
             element.valueChanged.connect(write_parameter)
 
         for param_name in ("optimization_mod_freq", "optimization_mod_amp"):
 
             def optim_enabled_changed(_, param_name=param_name):
                 getattr(self.parameters, param_name + "_enabled").value = int(
-                    getattr(self.ids, param_name).checkState()
+                    getattr(self, param_name).checkState()
                 )
 
-            getattr(self.ids, param_name).stateChanged.connect(optim_enabled_changed)
+            getattr(self, param_name).stateChanged.connect(optim_enabled_changed)
 
     def on_connection_established(self):
         self.parameters = self.app.parameters
         self.control = self.app.control
 
         def opt_running_changed(_):
             running = self.parameters.optimization_running.value
             approaching = self.parameters.optimization_approaching.value
             failed = self.parameters.optimization_failed.value
 
-            self.ids.optimization_not_running_container.setVisible(
+            self.optimization_not_running_container.setVisible(
                 not failed and not running
             )
-            self.ids.optimization_running_container.setVisible(
+            self.optimization_running_container.setVisible(
                 not failed and running and not approaching
             )
-            self.ids.optimization_preparing.setVisible(
+            self.optimization_preparing.setVisible(
                 not failed and running and approaching
             )
-            self.ids.optimization_failed.setVisible(failed)
+            self.optimization_failed.setVisible(failed)
 
-        self.parameters.optimization_running.on_change(opt_running_changed)
-        self.parameters.optimization_approaching.on_change(opt_running_changed)
-        self.parameters.optimization_failed.on_change(opt_running_changed)
+        self.parameters.optimization_running.add_callback(opt_running_changed)
+        self.parameters.optimization_approaching.add_callback(opt_running_changed)
+        self.parameters.optimization_failed.add_callback(opt_running_changed)
 
         def opt_selection_changed(value):
-            self.ids.optimization_selecting.setVisible(value)
-            self.ids.optimization_not_selecting.setVisible(not value)
+            self.optimization_selecting.setVisible(value)
+            self.optimization_not_selecting.setVisible(not value)
 
-        self.parameters.optimization_selection.on_change(opt_selection_changed)
+        self.parameters.optimization_selection.add_callback(opt_selection_changed)
 
         def mod_param_changed(_):
             dual_channel = self.parameters.dual_channel.value
             channel = self.parameters.optimization_channel.value
             optimized = self.parameters.optimization_optimized_parameters.value
 
-            self.ids.optimization_display_parameters.setText(
+            self.optimization_display_parameters.setText(
                 (
                     "<br />\n"
                     "<b>current parameters</b>: "
                     " %.2f&nbsp;MHz, %.2f&nbsp;Vpp, %.2f&nbsp;deg<br />\n"
                     "<b>optimized parameters</b>: "
                     "%.2f&nbsp;MHz, %.2f&nbsp;Vpp, %.2f&nbsp;deg\n"
                     "<br />"
@@ -118,64 +115,64 @@
                     )[0 if not dual_channel else (0, 1)[channel]].value,
                     optimized[0] / MHz,
                     optimized[1] / Vpp,
                     optimized[2],
                 )
             )
 
-        for p in (
+        for param in (
             self.parameters.modulation_amplitude,
             self.parameters.modulation_frequency,
             self.parameters.demodulation_phase_a,
         ):
-            p.on_change(mod_param_changed)
+            param.add_callback(mod_param_changed)
 
         def improvement_changed(improvement):
-            self.ids.optimization_improvement.setText("%d %%" % (improvement * 100))
+            self.optimization_improvement.setText(f"{improvement * 100} %%")
 
-        self.parameters.optimization_improvement.on_change(improvement_changed)
+        self.parameters.optimization_improvement.add_callback(improvement_changed)
 
         param2ui(
             self.parameters.optimization_mod_freq_enabled,
-            self.ids.optimization_mod_freq,
+            self.optimization_mod_freq,
         )
         param2ui(
             self.parameters.optimization_mod_freq_min,
-            self.ids.optimization_mod_freq_min,
+            self.optimization_mod_freq_min,
         )
         param2ui(
             self.parameters.optimization_mod_freq_max,
-            self.ids.optimization_mod_freq_max,
+            self.optimization_mod_freq_max,
         )
         param2ui(
-            self.parameters.optimization_mod_amp_enabled, self.ids.optimization_mod_amp
+            self.parameters.optimization_mod_amp_enabled, self.optimization_mod_amp
         )
         param2ui(
-            self.parameters.optimization_mod_amp_min, self.ids.optimization_mod_amp_min
+            self.parameters.optimization_mod_amp_min, self.optimization_mod_amp_min
         )
         param2ui(
-            self.parameters.optimization_mod_amp_max, self.ids.optimization_mod_amp_max
+            self.parameters.optimization_mod_amp_max, self.optimization_mod_amp_max
         )
 
         def dual_channel_changed(value):
-            self.ids.optimization_channel_selector_box.setVisible(value)
+            self.optimization_channel_selector_box.setVisible(value)
 
-        self.parameters.dual_channel.on_change(dual_channel_changed)
+        self.parameters.dual_channel.add_callback(dual_channel_changed)
 
         def fast_mode_changed(fast_mode_enabled):
             """Disable this panel if fast mode is enabled (nothing to optimize)."""
             self.setEnabled(not fast_mode_enabled)
 
-        self.parameters.fast_mode.on_change(fast_mode_changed)
+        self.parameters.fast_mode.add_callback(fast_mode_changed)
 
         def fast_mode_changed(fast_mode_enabled):
             """Disable this panel if fast mode is enabled (nothing to optimize)."""
             self.setEnabled(not fast_mode_enabled)
 
-        self.parameters.fast_mode.on_change(fast_mode_changed)
+        self.parameters.fast_mode.add_callback(fast_mode_changed)
 
     def start_optimization(self):
         self.parameters.optimization_selection.value = True
 
     def abort_selection(self):
         self.parameters.optimization_selection.value = False
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/optimization_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/optimization_panel.ui`

 * *Files 1% similar despite different names*

#### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/optimization_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/optimization_panel.ui`

```diff
@@ -3,15 +3,15 @@
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>400</width>
-        <height>1261</height>
+        <height>1086</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout_2">
       <item>
@@ -192,15 +192,15 @@
                             </property>
                             <property name="wordWrap">
                               <bool>true</bool>
                             </property>
                           </widget>
                         </item>
                         <item>
-                          <widget class="QComboBox" name="optimization_channel_selector">
+                          <widget class="QComboBox" name="optimizationChannelComboBox">
                             <property name="sizePolicy">
                               <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
                                 <horstretch>0</horstretch>
                                 <verstretch>0</verstretch>
                               </sizepolicy>
                             </property>
                             <item>
@@ -215,15 +215,15 @@
                             </item>
                           </widget>
                         </item>
                       </layout>
                     </widget>
                   </item>
                   <item>
-                    <widget class="QPushButton" name="start_optimization_btn">
+                    <widget class="QPushButton" name="startOptimizationPushButton">
                       <property name="minimumSize">
                         <size>
                           <width>0</width>
                           <height>50</height>
                         </size>
                       </property>
                       <property name="font">
@@ -336,15 +336,15 @@
                 </property>
                 <property name="wordWrap">
                   <bool>true</bool>
                 </property>
               </widget>
             </item>
             <item>
-              <widget class="QPushButton" name="optimization_use_new_parameters">
+              <widget class="QPushButton" name="useOptimizedParametersPushButton">
                 <property name="minimumSize">
                   <size>
                     <width>0</width>
                     <height>50</height>
                   </size>
                 </property>
                 <property name="font">
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/plot_widget.py` & `linien-gui-0.8.0rc1/linien_gui/ui/plot_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,17 +28,16 @@
     check_plot_data,
     combine_error_signal,
     determine_shift_by_correlation,
     get_lock_point,
     get_signal_strength_from_i_q,
     update_signal_history,
 )
-from linien_common.config import N_COLORS
-from linien_gui.config import DEFAULT_PLOT_RATE_LIMIT, Color
-from linien_gui.widgets import CustomWidget
+from linien_gui.config import DEFAULT_PLOT_RATE_LIMIT, N_COLORS, Color
+from linien_gui.utils import get_linien_app_instance
 from PyQt5 import QtGui, QtWidgets
 from PyQt5.QtCore import pyqtSignal
 from pyqtgraph.Qt import QtCore
 
 # NOTE: this is required for using a pen_width > 1. There is a bug though that causes
 # the plot to be way too small. Therefore, we call PlotWidget.resize() after a while
 pg.setConfigOptions(
@@ -56,49 +55,39 @@
 INVALID_POWER = -1000
 
 
 def peak_voltage_to_dBm(voltage):
     return 10 + 20 * np.log10(voltage)
 
 
-class TimeXAxis(pg.AxisItem, CustomWidget):
+class TimeXAxis(pg.AxisItem):
     """Plots x axis as time in seconds instead of point number."""
 
     def __init__(self, *args, parent=None, **kwargs):
         pg.AxisItem.__init__(self, *args, **kwargs)
         self.parent = parent
-
-    @property
-    def parameters(self):
-        return self.parent.parameters
-
-    @property
-    def sweep_speed(self):
-        return self.parameters.sweep_speed
-
-    @property
-    def lock(self):
-        return self.parameters.lock
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
 
     def on_connection_established(self):
         # we have to wait until parameters (of parent) is available
         QtCore.QTimer.singleShot(100, self.listen_to_parameter_changes)
 
     def listen_to_parameter_changes(self):
-        self.sweep_speed.on_change(self.force_repaint_tick_strings)
-        self.lock.on_change(self.force_repaint_tick_strings)
+        self.parent.parameters.sweep_speed.add_callback(self.force_repaint_tick_strings)
+        self.parent.parameters.lock.add_callback(self.force_repaint_tick_strings)
         self.force_repaint_tick_strings()
 
     def force_repaint_tick_strings(self, *args):
         self.picture = None
         self.update()
 
     def tickStrings(self, values, scale, spacing):
-        locked = self.lock.value
-        sweep_speed = self.sweep_speed.value if not locked else 0
+        locked = self.parent.parameters.lock.value
+        sweep_speed = self.parent.parameters.sweep_speed.value if not locked else 0
         time_between_points = (1 / 125e6) * 2 ** (sweep_speed) * DECIMATION
         values = [v * time_between_points for v in values]
         spacing *= time_between_points
 
         places = max(0, np.ceil(-np.log10(spacing * scale)))
         strings = []
         for v in values:
@@ -107,28 +96,29 @@
                 vstr = "%g" % vs
             else:
                 vstr = ("%%0.%df" % places) % vs
             strings.append(vstr)
         return strings
 
 
-class PlotWidget(pg.PlotWidget, CustomWidget):
+class PlotWidget(pg.PlotWidget):
     signal_power1 = pyqtSignal(float)
     signal_power2 = pyqtSignal(float)
     keyPressed = pyqtSignal(int)
 
     def __init__(self, *args, **kwargs):
-        super().__init__(
+        super(PlotWidget, self).__init__(
             *args,
-            axisItems={"bottom": TimeXAxis(orientation="bottom", parent=self)},
+            axisItems={"bottom": TimeXAxis(parent=self, orientation="bottom")},
             **kwargs,
         )
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
 
         self.getAxis("bottom").enableAutoSIPrefix(False)
-
         self.showGrid(x=True, y=True)
         self.setLabel("bottom", "time", units="s")
 
         # Causes auto-scale button (‘A’ in lower-left corner) to be hidden for this
         # PlotItem
         self.hideButtons()
         # we have our own "reset view" button instead
@@ -212,77 +202,79 @@
         self.last_plot_time = 0
         self.plot_rate_limit = DEFAULT_PLOT_RATE_LIMIT
 
         self._plot_paused = False
         self._cached_plot_data = []
         self._should_reposition_reset_view_button = False
 
-    def _to_data_coords(self, event):
-        pos = self.plotItem.vb.mapSceneToView(event.pos())
-        x, y = pos.x(), pos.y()
-        return x, y
-
     def on_connection_established(self):
         self.parameters = self.app.parameters
         self.control = self.app.control
 
         def set_pens(*args):
-            pen_width = self.parameters.plot_line_width.value
+            pen_width = self.app.settings.plot_line_width.value
 
             for curve, color in {
                 self.signal1: Color.SPECTRUM1,
                 self.signal2: Color.SPECTRUM2,
                 self.combined_signal: Color.SPECTRUM_COMBINED,
                 self.control_signal: Color.CONTROL_SIGNAL,
                 self.control_signal_history: Color.CONTROL_SIGNAL_HISTORY,
                 self.slow_history: Color.SLOW_HISTORY,
                 self.monitor_signal_history: Color.MONITOR_SIGNAL_HISTORY,
             }.items():
-                r, g, b, *stuff = getattr(
-                    self.parameters, f"plot_color_{color.value}"
+                r, g, b, _ = getattr(
+                    self.app.settings, f"plot_color_{color.value}"
                 ).value
-                a = self.parameters.plot_line_opacity.value
+                a = self.app.settings.plot_line_opacity.value
                 curve.setPen(pg.mkPen((r, g, b, a), width=pen_width))
 
         for color_idx in range(N_COLORS):
-            getattr(self.parameters, "plot_color_%d" % color_idx).on_change(set_pens)
-        self.parameters.plot_line_width.on_change(set_pens)
-        self.parameters.plot_line_opacity.on_change(set_pens)
+            getattr(self.app.settings, f"plot_color_{color_idx}").add_callback(set_pens)
+        self.app.settings.plot_line_width.add_callback(set_pens)
+        self.app.settings.plot_line_opacity.add_callback(set_pens)
 
         self.control_signal_history_data = self.parameters.control_signal_history.value
         self.monitor_signal_history_data = self.parameters.monitor_signal_history.value
 
-        self.parameters.to_plot.on_change(self.replot)
+        self.parameters.to_plot.add_callback(self.replot)
 
         def autolock_selection_changed(value):
             if value:
                 self.parameters.optimization_selection.value = False
                 self.enable_area_selection(selectable_width=0.99)
                 self.pause_plot_and_cache_data()
             elif not self.parameters.optimization_selection.value:
                 self.disable_area_selection()
                 self.resume_plot_and_clear_cache()
 
-        self.parameters.autolock_selection.on_change(autolock_selection_changed)
+        self.parameters.autolock_selection.add_callback(autolock_selection_changed)
 
         def optimization_selection_changed(value):
             if value:
                 self.parameters.autolock_selection.value = False
                 self.enable_area_selection(selectable_width=0.75)
                 self.pause_plot_and_cache_data()
             elif not self.parameters.autolock_selection.value:
                 self.disable_area_selection()
                 self.resume_plot_and_clear_cache()
 
-        self.parameters.optimization_selection.on_change(optimization_selection_changed)
+        self.parameters.optimization_selection.add_callback(
+            optimization_selection_changed
+        )
 
         def show_or_hide_crosshair(automatic_mode):
             self.crosshair.setVisible(not automatic_mode)
 
-        self.parameters.automatic_mode.on_change(show_or_hide_crosshair)
+        self.parameters.automatic_mode.add_callback(show_or_hide_crosshair)
+
+    def _to_data_coords(self, event):
+        pos = self.plotItem.vb.mapSceneToView(event.pos())
+        x, y = pos.x(), pos.y()
+        return x, y
 
     def mouseMoveEvent(self, event):
         if not self.selection_running:
             super().mouseMoveEvent(event)
         else:
             if self.touch_start is None:
                 return
@@ -526,15 +518,15 @@
                             self.plot_signal_strength(
                                 s1,
                                 s1q,
                                 self.signal_strength_a,
                                 self.signal_strength_a2,
                                 self.signal_strength_a_fill,
                                 self.parameters.offset_a.value,
-                                self.parameters.plot_color_0.value,
+                                self.app.settings.plot_color_0.value,
                             )
                             / V
                         )
                         all_signals.append(
                             [
                                 max_signal_strength_V * V,
                                 -1 * max_signal_strength_V * V,
@@ -552,15 +544,15 @@
                             self.plot_signal_strength(
                                 s2,
                                 s2q,
                                 self.signal_strength_b,
                                 self.signal_strength_b2,
                                 self.signal_strength_b_fill,
                                 self.parameters.offset_b.value,
-                                self.parameters.plot_color_1.value,
+                                self.app.settings.plot_color_1.value,
                             )
                             / V
                         )
 
                         all_signals.append(
                             [
                                 max_signal_strength2_V * V,
@@ -604,15 +596,15 @@
         r, g, b, *stuff = color
 
         x = list(range(len(signal_strength)))
         signal_strength_scaled = signal_strength / V
         upper = (channel_offset / V) + signal_strength_scaled
         lower = (channel_offset / V) - 1 * signal_strength_scaled
 
-        brush = pg.mkBrush(r, g, b, self.parameters.plot_fill_opacity.value)
+        brush = pg.mkBrush(r, g, b, self.app.settings.plot_fill_opacity.value)
         fill.setBrush(brush)
 
         invisible_pen = pg.mkPen("k", width=0.00001)
         signal.setData(x, upper, pen=invisible_pen)
         neg_signal.setData(x, lower, pen=invisible_pen)
         return np.max([np.max(upper), -1 * np.min(lower)]) * V
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/psd_plot_widget.py` & `linien-gui-0.8.0rc1/linien_gui/ui/psd_plot_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import numpy as np
 import pyqtgraph as pg
 from linien_gui.ui.plot_widget import V
-from linien_gui.widgets import CustomWidget
+from linien_gui.utils import get_linien_app_instance
 
 
 class CustomLogAxis(pg.AxisItem):
     """This class overrides the tick label generator function of the default
     axis. It reimplements it such that negative exponents are also displayed
     in scientific notation."""
 
@@ -69,24 +69,26 @@
                 dstrings.append(v + "10" + sign + pot)
             else:
                 dstrings.append(e)
 
         return dstrings
 
 
-class PSDPlotWidget(pg.PlotWidget, CustomWidget):
+class PSDPlotWidget(pg.PlotWidget):
     def __init__(self, *args, **kwargs):
-        super().__init__(
+        super(PSDPlotWidget, self).__init__(
             *args,
             axisItems={
                 "bottom": CustomLogAxis(orientation="bottom"),
                 "left": CustomLogAxis(orientation="left"),
             },
             **kwargs
         )
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
 
         self.curves = {}
 
         self.setLogMode(x=True, y=True)
         self.setLabel("left", "PSD", units="V / Sqrt[Hz]")
         self.setLabel("bottom", "Frequency", units="Hz")
         self.getAxis("left").enableAutoSIPrefix(False)
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/psd_table_widget.py` & `linien-gui-0.8.0rc1/linien_gui/ui/psd_table_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime
 
-from linien_gui.utils import color_to_hex
-from linien_gui.widgets import CustomWidget
+from linien_gui.utils import color_to_hex, get_linien_app_instance
 from PyQt5 import QtCore, QtWidgets
 from PyQt5.QtCore import pyqtSignal
 
 
-class PSDTableWidget(QtWidgets.QTableWidget, CustomWidget):
+class PSDTableWidget(QtWidgets.QTableWidget):
     show_or_hide_curve = pyqtSignal(str, bool)
 
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super(PSDTableWidget, self).__init__(*args, **kwargs)
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
 
         self.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
         self.setSizeAdjustPolicy(QtWidgets.QAbstractScrollArea.AdjustToContents)
 
         self.uuids = []
 
     def on_connection_established(self):
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/psd_window.py` & `linien-gui-0.8.0rc1/linien_gui/ui/psd_window.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,96 +18,100 @@
 
 import pickle
 from time import time
 
 import linien_gui
 from linien_common.common import PSD_ALGORITHM_LPSD, PSD_ALGORITHM_WELCH
 from linien_gui.dialogs import error_dialog
-from linien_gui.utils import RandomColorChoser, param2ui, set_window_icon
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import (
+    RandomColorChoser,
+    get_linien_app_instance,
+    param2ui,
+    set_window_icon,
+)
+from linien_gui.widgets import UI_PATH
+from PyQt5 import QtWidgets, uic
 
 
-class PSDWindow(QtWidgets.QMainWindow, CustomWidget):
+class PSDWindow(QtWidgets.QMainWindow):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.load_ui("psd_window.ui")
+        super(PSDWindow, self).__init__(*args, **kwargs)
+        uic.loadUi(UI_PATH / "psd_window.ui", self)
         self.setWindowTitle("Linien: Noise analysis")
         set_window_icon(self)
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
+
         self.random_color_choser = RandomColorChoser()
         self.colors = {}
         self.data = {}
         self.complete_uids = []
 
-    def ready(self):
-        self.ids.start_psd_button.clicked.connect(self.start_psd)
-        """self.ids.start_pid_optimization_button.clicked.connect(
-            self.start_pid_optimization
-        )"""
-        self.ids.stop_psd_button.clicked.connect(self.stop_psd)
-
-        self.ids.curve_table.show_or_hide_curve.connect(
-            self.ids.psd_plot_widget.show_or_hide_curve
-        )
-        self.ids.delete_curve_button.clicked.connect(self.delete_curve)
-        self.ids.export_psd_button.clicked.connect(self.export_psd)
-        self.ids.import_psd_button.clicked.connect(self.import_psd)
+        self.start_psd_button.clicked.connect(self.start_psd)
+        self.stop_psd_button.clicked.connect(self.stop_psd)
 
-        self.ids.maximum_measurement_time.currentIndexChanged.connect(
-            self.change_maximum_measurement_time
+        self.curve_table.show_or_hide_curve.connect(
+            self.psd_plot_widget.show_or_hide_curve
         )
+        self.delete_curve_button.clicked.connect(self.delete_curve)
+        self.export_psd_button.clicked.connect(self.export_psd)
+        self.import_psd_button.clicked.connect(self.import_psd)
 
-        self.ids.psd_algorithm.currentIndexChanged.connect(self.change_psd_algorithm)
-
-    def closeEvent(self, event, *args, **kwargs):
-        # we never realy want to close the window (which destroys its content)
-        # but just to hide it
-        event.ignore()
-        self.hide()
+        self.maximum_measurement_time.currentIndexChanged.connect(
+            self.change_maximum_measurement_time
+        )
 
-    def change_maximum_measurement_time(self, index):
-        self.parameters.psd_acquisition_max_decimation.value = 12 + index
-
-    def change_psd_algorithm(self, index):
-        self.parameters.psd_algorithm.value = [PSD_ALGORITHM_LPSD, PSD_ALGORITHM_WELCH][
-            index
-        ]
+        self.psd_algorithm.currentIndexChanged.connect(self.change_psd_algorithm)
 
     def on_connection_established(self):
         self.parameters = self.app.parameters
         self.control = self.app.control
 
-        self.parameters.psd_data_partial.on_change(
+        self.parameters.psd_data_partial.add_callback(
             self.psd_data_received,
         )
-        self.parameters.psd_data_complete.on_change(
+        self.parameters.psd_data_complete.add_callback(
             self.psd_data_received,
         )
 
         param2ui(
             self.parameters.psd_acquisition_max_decimation,
-            self.ids.maximum_measurement_time,
+            self.maximum_measurement_time,
             lambda max_decimation: max_decimation - 12,
         )
         param2ui(
             self.parameters.psd_algorithm,
-            self.ids.psd_algorithm,
+            self.psd_algorithm,
             lambda algo: {PSD_ALGORITHM_LPSD: 0, PSD_ALGORITHM_WELCH: 1}[algo],
         )
 
         def update_status(_):
             psd_running = self.parameters.psd_acquisition_running.value
             if psd_running:
-                self.ids.container_psd_running.show()
-                self.ids.container_psd_not_running.hide()
+                self.container_psd_running.show()
+                self.container_psd_not_running.hide()
             else:
-                self.ids.container_psd_running.hide()
-                self.ids.container_psd_not_running.show()
+                self.container_psd_running.hide()
+                self.container_psd_not_running.show()
+
+        self.parameters.psd_acquisition_running.add_callback(update_status)
 
-        self.parameters.psd_acquisition_running.on_change(update_status)
+    def closeEvent(self, event, *args, **kwargs):
+        # we never realy want to close the window (which destroys its content)  but just
+        # to hide it
+        event.ignore()
+        self.hide()
+
+    def change_maximum_measurement_time(self, index):
+        self.parameters.psd_acquisition_max_decimation.value = 12 + index
+
+    def change_psd_algorithm(self, index):
+        self.parameters.psd_algorithm.value = [PSD_ALGORITHM_LPSD, PSD_ALGORITHM_WELCH][
+            index
+        ]
 
     def psd_data_received(self, data_pickled):
         if data_pickled is None:
             return
 
         data = pickle.loads(data_pickled)
 
@@ -126,16 +130,16 @@
         # or generate a new color if the curve was not yet partially plotted
         if curve_uuid not in self.colors:
             color = self.random_color_choser.get()
             self.colors[curve_uuid] = color
         else:
             color = self.colors[curve_uuid]
 
-        self.ids.psd_plot_widget.plot_curve(curve_uuid, data["psds"], color)
-        self.ids.curve_table.add_curve(curve_uuid, data, color)
+        self.psd_plot_widget.plot_curve(curve_uuid, data["psds"], color)
+        self.curve_table.add_curve(curve_uuid, data, color)
 
         self.data[curve_uuid] = data
 
     def start_psd(self):
         if not self.parameters.lock.value:
             return error_dialog(self, """Laser has to be locked for PSD measurement!""")
 
@@ -146,17 +150,17 @@
             self.parameters.task.value.stop()
             self.parameters.task.value = None
 
     def start_pid_optimization(self):
         self.control.start_pid_optimization()
 
     def delete_curve(self):
-        uuid = self.ids.curve_table.delete_selected_curve()
+        uuid = self.curve_table.delete_selected_curve()
         if uuid is not None:
-            self.ids.psd_plot_widget.delete_curve(uuid)
+            self.psd_plot_widget.delete_curve(uuid)
             del self.data[uuid]
 
     def export_psd(self):
         options = QtWidgets.QFileDialog.Options()
         # options |= QtWidgets.QFileDialog.DontUseNativeDialog
         default_ext = ".pickle"
         fn, _ = QtWidgets.QFileDialog.getSaveFileName(
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/psd_window.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/psd_window.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/right_panel.py` & `linien-gui-0.8.0rc1/linien_gui/ui/right_panel.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,74 +12,81 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import get_linien_app_instance
+from PyQt5 import QtCore, QtWidgets
 
 
-class RightPanel(QtWidgets.QWidget, CustomWidget):
+class RightPanel(QtWidgets.QWidget):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super(RightPanel, self).__init__(*args, **kwargs)
+        self.app = get_linien_app_instance()
+        self.app.connection_established.connect(self.on_connection_established)
+        self.main_window = self.window()
+        QtCore.QTimer.singleShot(100, self.ready)
+
+    def ready(self):
+        self.main_window.closeButton.clicked.connect(self.app.quit)
+        self.main_window.shutdownButton.clicked.connect(self.shutdown_server)
+        self.main_window.openDeviceManagerButton.clicked.connect(
+            self.open_device_manager
+        )
+        self.main_window.pid_parameter_optimization_button.clicked.connect(
+            self.open_psd_window
+        )
 
     def on_connection_established(self):
         self.parameters = self.app.parameters
         self.control = self.app.control
 
-        self.parameters.autolock_running.on_change(self.autolock_status_changed)
-        self.parameters.optimization_running.on_change(self.optimization_status_changed)
-        self.parameters.lock.on_change(self.enable_or_disable_panels)
+        self.parameters.autolock_running.add_callback(self.autolock_status_changed)
+        self.parameters.optimization_running.add_callback(
+            self.optimization_status_changed
+        )
+        self.parameters.lock.add_callback(self.enable_or_disable_panels)
 
         def highlight_psd_button(locked):
-            self.ids.pid_parameter_optimization_button.setStyleSheet(
+            self.main_window.pid_parameter_optimization_button.setStyleSheet(
                 "background: #00aa00;" if locked else ""
             )
 
-        self.parameters.lock.on_change(highlight_psd_button)
-
-    def ready(self):
-        self.ids.closeButton.clicked.connect(self.close_app)
-        self.ids.shutdownButton.clicked.connect(self.shutdown_server)
-        self.ids.openDeviceManagerButton.clicked.connect(self.open_device_manager)
-        self.ids.pid_parameter_optimization_button.clicked.connect(self.open_psd_window)
-
-    def close_app(self):
-        self.app.close()
+        self.parameters.lock.add_callback(highlight_psd_button)
 
     def shutdown_server(self):
         self.app.shutdown()
 
     def open_psd_window(self):
         self.app.open_psd_window()
 
     def open_device_manager(self):
         self.app.open_device_manager()
 
     def autolock_status_changed(self, value):
         if value:
-            self.ids.settings_toolbox.setCurrentWidget(self.ids.lockingPanel)
+            self.main_window.settings_toolbox.setCurrentWidget(self.lockingPanel)
 
         self.enable_or_disable_panels()
 
     def optimization_status_changed(self, value):
         if value:
-            self.ids.settings_toolbox.setCurrentWidget(self.ids.optimizationPanel)
+            self.main_window.settings_toolbox.setCurrentWidget(self.optimizationPanel)
 
         self.enable_or_disable_panels()
 
     def enable_or_disable_panels(self, *args):
         lock = self.parameters.lock.value
         autolock = self.parameters.autolock_running.value
         optimization = self.parameters.optimization_running.value
 
         def enable_panels(panel_names, condition):
             for panel_name in panel_names:
-                getattr(self.ids, panel_name).setEnabled(condition)
+                getattr(self.main_window, panel_name).setEnabled(condition)
 
         enable_panels(("generalPanel",), not autolock and not optimization and not lock)
         enable_panels(
             ("modSpectroscopyPanel", "viewPanel", "lockingPanel"), not optimization
         )
         enable_panels(("optimizationPanel",), not autolock and not lock)
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/spectroscopy_panel.py` & `linien-gui-0.8.0rc1/linien_gui/ui/spectroscopy_panel.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,146 +12,150 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
+from typing import Union
+
+from linien_client.remote_parameters import RemoteParameter
 from linien_common.common import HIGH_PASS_FILTER, LOW_PASS_FILTER
-from linien_gui.utils import param2ui
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import get_linien_app_instance, param2ui
+from linien_gui.widgets import UI_PATH
+from PyQt5 import QtWidgets, uic
+
 
+class SpectroscopyPanel(QtWidgets.QWidget):
+    CHANNEL = Union[str, None]
 
-class SpectroscopyPanel(QtWidgets.QWidget, CustomWidget):
     def __init__(self, *args):
-        super().__init__(*args)
-        self.load_ui("spectroscopy_panel.ui")
+        super(SpectroscopyPanel, self).__init__(*args)
+        uic.loadUi(UI_PATH / "spectroscopy_panel.ui", self)
+        self.app = get_linien_app_instance()
 
         def change_filter_frequency(filter_i):
-            self.get_param("filter_%d_frequency" % filter_i).value = getattr(
-                self.ids, "filter_%d_frequency" % filter_i
+            self.get_param(f"filter_{filter_i}_frequency").value = getattr(
+                self, f"filter_{filter_i}_frequency"
             ).value()
-            self.control.write_registers()
+            self.control.exposed_write_registers()
 
         def change_filter_enabled(filter_i):
             filter_enabled = int(
-                getattr(self.ids, "filter_%d_enabled" % filter_i).checkState() > 0
+                getattr(self, f"filter_{filter_i}_enabled").checkState() > 0
             )
-            self.get_param("filter_%d_enabled" % filter_i).value = filter_enabled
-            self.control.write_registers()
+            self.get_param(f"filter_{filter_i}_enabled").value = filter_enabled
+            self.control.exposed_write_registers()
 
         def change_filter_type(filter_i):
-            param = self.get_param("filter_%d_type" % filter_i)
-            current_idx = getattr(self.ids, "filter_%d_type" % filter_i).currentIndex()
+            param = self.get_param(f"filter_{filter_i}_type")
+            current_idx = getattr(self, f"filter_{filter_i}_type").currentIndex()
             param.value = (LOW_PASS_FILTER, HIGH_PASS_FILTER)[current_idx]
-            self.control.write_registers()
+            self.control.exposed_write_registers()
 
         for filter_i in [1, 2]:
             for key, fct in {
-                "change_filter_%d_frequency": change_filter_frequency,
-                "change_filter_%d_enabled": change_filter_enabled,
-                "change_filter_%d_type": change_filter_type,
+                f"change_filter_{filter_i}_frequency": change_filter_frequency,
+                f"change_filter_{filter_i}_enabled": change_filter_enabled,
+                f"change_filter_{filter_i}_type": change_filter_type,
             }.items():
                 setattr(
                     self,
-                    key % filter_i,
+                    key,
                     lambda *args, fct=fct, filter_i=filter_i: fct(filter_i),
                 )
 
-    def get_param(self, name):
-        return getattr(
-            self.parameters, "%s_%s" % (name, "a" if self.channel == 0 else "b")
-        )
-
-    def ready(self):
-        self.ids.signal_offset.setKeyboardTracking(False)
-        self.ids.signal_offset.valueChanged.connect(self.change_signal_offset)
-        self.ids.demodulation_phase.setKeyboardTracking(False)
-        self.ids.demodulation_phase.valueChanged.connect(self.change_demod_phase)
-        self.ids.demodulation_frequency.currentIndexChanged.connect(
+        self.signalOffsetSpinBox.setKeyboardTracking(False)
+        self.signalOffsetSpinBox.valueChanged.connect(self.change_signal_offset)
+        self.demodulationPhaseSpinBox.setKeyboardTracking(False)
+        self.demodulationPhaseSpinBox.valueChanged.connect(self.change_demod_phase)
+        self.demodulationFrequencyComboBox.currentIndexChanged.connect(
             self.change_demod_multiplier
         )
 
         for filter_i in [1, 2]:
             _get = lambda parent, attr, filter_i=filter_i: getattr(
-                parent, attr % filter_i
+                parent, attr.format(filter_i)
             )
-            _get(self.ids, "filter_%d_enabled").stateChanged.connect(
-                _get(self, "change_filter_%d_enabled")
+            _get(self, "filter_{}_enabled").stateChanged.connect(
+                _get(self, "change_filter_{}_enabled")
             )
-            freq_input = _get(self.ids, "filter_%d_frequency")
+            freq_input = _get(self, "filter_{}_frequency")
             freq_input.setKeyboardTracking(False)
-            freq_input.valueChanged.connect(_get(self, "change_filter_%d_frequency"))
-            _get(self.ids, "filter_%d_type").currentIndexChanged.connect(
-                _get(self, "change_filter_%d_type")
+            freq_input.valueChanged.connect(_get(self, "change_filter_{}_frequency"))
+            _get(self, "filter_{}_type").currentIndexChanged.connect(
+                _get(self, "change_filter_{}_type")
             )
 
         def automatic_changed(value):
             self.get_param("filter_automatic").value = value
-            self.control.write_registers()
+            self.control.exposed_write_registers()
 
-        self.ids.filter_automatic.stateChanged.connect(automatic_changed)
+        self.automaticFilterCheckBox.stateChanged.connect(automatic_changed)
 
         def invert_changed(value):
             self.get_param("invert").value = bool(value)
-            self.control.write_registers()
+            self.control.exposed_write_registers()
 
-        self.ids.invert.stateChanged.connect(invert_changed)
+        self.invertCheckBox.stateChanged.connect(invert_changed)
 
     def on_connection_established(self):
         self.parameters = self.app.parameters
         self.control = self.app.control
 
-        # self.close_button.clicked.connect(self.close_app)
-        # self.shutdown_button.clicked.connect(self.shutdown_server)
-
-        param2ui(self.get_param("demodulation_phase"), self.ids.demodulation_phase)
+        param2ui(self.get_param("demodulation_phase"), self.demodulationPhaseSpinBox)
         param2ui(
             self.get_param("demodulation_multiplier"),
-            self.ids.demodulation_frequency,
+            self.demodulationFrequencyComboBox,
             lambda value: value - 1,
         )
-        param2ui(self.get_param("offset"), self.ids.signal_offset, lambda v: v / 8191.0)
-        param2ui(self.get_param("invert"), self.ids.invert)
-        param2ui(self.get_param("filter_automatic"), self.ids.filter_automatic)
+        param2ui(
+            self.get_param("offset"), self.signalOffsetSpinBox, lambda v: v / 8191.0
+        )
+        param2ui(self.get_param("invert"), self.invertCheckBox)
+        param2ui(self.get_param("filter_automatic"), self.automaticFilterCheckBox)
 
         def filter_automatic_changed(value):
-            self.ids.automatic_filtering_enabled.setVisible(value)
-            self.ids.automatic_filtering_disabled.setVisible(not value)
+            self.automatic_filtering_enabled.setVisible(value)
+            self.automatic_filtering_disabled.setVisible(not value)
 
-        self.get_param("filter_automatic").on_change(filter_automatic_changed)
+        self.get_param("filter_automatic").add_callback(filter_automatic_changed)
 
         for filter_i in [1, 2]:
             param2ui(
-                self.get_param("filter_%d_enabled" % filter_i),
-                getattr(self.ids, "filter_%d_enabled" % filter_i),
+                self.get_param(f"filter_{filter_i}_enabled"),
+                getattr(self, f"filter_{filter_i}_enabled"),
             )
             param2ui(
-                self.get_param("filter_%d_frequency" % filter_i),
-                getattr(self.ids, "filter_%d_frequency" % filter_i),
+                self.get_param(f"filter_{filter_i}_frequency"),
+                getattr(self, f"filter_{filter_i}_frequency"),
             )
             param2ui(
-                self.get_param("filter_%d_type" % filter_i),
-                getattr(self.ids, "filter_%d_type" % filter_i),
+                self.get_param(f"filter_{filter_i}_type"),
+                getattr(self, f"filter_{filter_i}_type"),
                 lambda type_: {LOW_PASS_FILTER: 0, HIGH_PASS_FILTER: 1}[type_],
             )
 
+    def get_param(self, name: str) -> RemoteParameter:
+        return getattr(self.parameters, f"{name}_{self.CHANNEL}")
+
     def change_signal_offset(self):
-        self.get_param("offset").value = self.ids.signal_offset.value() * 8191
-        self.control.write_registers()
+        self.get_param("offset").value = self.signalOffsetSpinBox.value() * 8191
+        self.control.exposed_write_registers()
 
     def change_demod_phase(self):
-        self.get_param("demodulation_phase").value = self.ids.demodulation_phase.value()
-        self.control.write_registers()
+        self.get_param(
+            "demodulation_phase"
+        ).value = self.demodulationPhaseSpinBox.value()
+        self.control.exposed_write_registers()
 
     def change_demod_multiplier(self, idx):
         self.get_param("demodulation_multiplier").value = idx + 1
-        self.control.write_registers()
+        self.control.exposed_write_registers()
 
 
 class SpectroscopyChannelAPanel(SpectroscopyPanel):
-    channel = 0
+    CHANNEL = "a"
 
 
 class SpectroscopyChannelBPanel(SpectroscopyPanel):
-    channel = 1
+    CHANNEL = "b"
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/spectroscopy_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/spectroscopy_panel.ui`

 * *Files 2% similar despite different names*

#### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/spectroscopy_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/spectroscopy_panel.ui`

```diff
@@ -3,15 +3,15 @@
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>292</width>
-        <height>807</height>
+        <height>814</height>
       </rect>
     </property>
     <property name="sizePolicy">
       <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
         <horstretch>0</horstretch>
         <verstretch>0</verstretch>
       </sizepolicy>
@@ -31,15 +31,15 @@
           <property name="title">
             <string>Demodulation frequency</string>
           </property>
           <layout class="QVBoxLayout" name="verticalLayout_13">
             <item>
               <layout class="QHBoxLayout" name="horizontalLayout_5">
                 <item>
-                  <widget class="QComboBox" name="demodulation_frequency">
+                  <widget class="QComboBox" name="demodulationFrequencyComboBox">
                     <property name="styleSheet">
                       <string notr="true"/>
                     </property>
                     <item>
                       <property name="text">
                         <string>1f</string>
                       </property>
@@ -83,15 +83,15 @@
           <property name="title">
             <string>Demodulation phase</string>
           </property>
           <layout class="QVBoxLayout" name="verticalLayout_3">
             <item>
               <layout class="QHBoxLayout" name="horizontalLayout_4">
                 <item>
-                  <widget class="CustomDoubleSpinBoxNoSign" name="demodulation_phase">
+                  <widget class="CustomDoubleSpinBoxNoSign" name="demodulationPhaseSpinBox">
                     <property name="maximum">
                       <double>360.000000000000000</double>
                     </property>
                     <property name="singleStep">
                       <double>10.000000000000000</double>
                     </property>
                   </widget>
@@ -113,15 +113,15 @@
           <property name="title">
             <string>Signal offset</string>
           </property>
           <layout class="QHBoxLayout" name="horizontalLayout_7">
             <item>
               <layout class="QHBoxLayout" name="horizontalLayout_3">
                 <item>
-                  <widget class="CustomDoubleSpinBox" name="signal_offset">
+                  <widget class="CustomDoubleSpinBox" name="signalOffsetSpinBox">
                     <property name="decimals">
                       <number>3</number>
                     </property>
                     <property name="minimum">
                       <double>-1.000000000000000</double>
                     </property>
                     <property name="maximum">
@@ -153,15 +153,15 @@
       <item>
         <widget class="QGroupBox" name="filtering_group">
           <property name="title">
             <string>Filtering</string>
           </property>
           <layout class="QVBoxLayout" name="verticalLayout_2">
             <item>
-              <widget class="QCheckBox" name="filter_automatic">
+              <widget class="QCheckBox" name="automaticFilterCheckBox">
                 <property name="text">
                   <string>Automatic</string>
                 </property>
               </widget>
             </item>
             <item>
               <widget class="QLabel" name="automatic_filtering_enabled">
@@ -358,34 +358,34 @@
       <item>
         <widget class="QGroupBox" name="groupBox">
           <property name="title">
             <string>Invert</string>
           </property>
           <layout class="QVBoxLayout" name="verticalLayout_4">
             <item>
-              <widget class="QCheckBox" name="invert">
+              <widget class="QCheckBox" name="invertCheckBox">
                 <property name="text">
                   <string>Invert the signal</string>
                 </property>
               </widget>
             </item>
           </layout>
         </widget>
       </item>
     </layout>
   </widget>
   <customwidgets>
     <customwidget>
-      <class>CustomSpinBox</class>
-      <extends>QSpinBox</extends>
+      <class>CustomDoubleSpinBoxNoSign</class>
+      <extends>QDoubleSpinBox</extends>
       <header location="global">spin_box.h</header>
     </customwidget>
     <customwidget>
-      <class>CustomDoubleSpinBoxNoSign</class>
-      <extends>QDoubleSpinBox</extends>
+      <class>CustomSpinBox</class>
+      <extends>QSpinBox</extends>
       <header location="global">spin_box.h</header>
     </customwidget>
     <customwidget>
       <class>CustomDoubleSpinBox</class>
       <extends>QDoubleSpinBox</extends>
       <header location="global">spin_box.h</header>
     </customwidget>
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/spin_box.py` & `linien-gui-0.8.0rc1/linien_gui/ui/spin_box.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/sweep_control.py` & `linien-gui-0.8.0rc1/linien_gui/ui/sweep_control.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,69 +12,78 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import superqt
-from linien_gui.widgets import CustomWidget
-from PyQt5 import QtWidgets
+from linien_gui.utils import get_linien_app_instance
+from PyQt5 import QtCore, QtWidgets
 
 
-class SweepControlWidget(QtWidgets.QWidget, CustomWidget):
+class SweepControlWidget(QtWidgets.QWidget):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super(SweepControlWidget, self).__init__(*args, **kwargs)
+        self.app = get_linien_app_instance()
+        self.main_window = self.window()
+        self.app.connection_established.connect(self.on_connection_established)
+        QtCore.QTimer.singleShot(100, self.ready)
 
     def ready(self):
-        # initialize sweep slider boundaries
-        self.ids.sweep_slider.init()
+        self.main_window.sweepSlider.ready()  # initialize sweep slider boundaries
 
     def on_connection_established(self):
         self.control = self.app.control
         self.parameters = self.app.parameters
 
-        self.ids.sweep_slider.valueChanged.connect(self.update_sweep_range)
+        self.main_window.sweepSlider.valueChanged.connect(self.update_sweep_range)
         # NOTE: The keyboardTracking property of the QDoubleSpinBoxes has been set to
         # False, to avoid signal emission when editing the field. Signals are still
         # emitted when using the arrow buttons. See also the editingFinished method.
-        self.ids.sweep_center.valueChanged.connect(self.update_sweep_center)
-        self.ids.sweep_amplitude.valueChanged.connect(self.update_sweep_amplitude)
-        self.ids.sweep_start_stop_button.clicked.connect(self.pause_or_resume_sweep)
+        self.main_window.sweepCenterSpinBox.valueChanged.connect(
+            self.update_sweep_center
+        )
+        self.main_window.sweepAmplitudeSpinBox.valueChanged.connect(
+            self.update_sweep_amplitude
+        )
+        self.main_window.sweepStartStopPushButton.clicked.connect(
+            self.pause_or_resume_sweep
+        )
 
         # initialize sweep controls
         self.display_sweep_status()
 
         # change displayed values when sweep parameters change
-        self.parameters.sweep_center.on_change(self.display_sweep_status)
-        self.parameters.sweep_amplitude.on_change(self.display_sweep_status)
-        self.parameters.sweep_pause.on_change(self.display_sweep_status)
+        self.parameters.sweep_center.add_callback(self.display_sweep_status)
+        self.parameters.sweep_amplitude.add_callback(self.display_sweep_status)
+        self.parameters.sweep_pause.add_callback(self.display_sweep_status)
 
     def display_sweep_status(self, *args):
         center = self.parameters.sweep_center.value
         amplitude = self.parameters.sweep_amplitude.value
         min_ = center - amplitude
         max_ = center + amplitude
 
         # block signals to avoid infinite loops when changing sweep parameters, see also
         # param2ui
-        self.ids.sweep_slider.blockSignals(True)
-        self.ids.sweep_amplitude.blockSignals(True)
-        self.ids.sweep_center.blockSignals(True)
-
-        self.ids.sweep_slider.setValue((min_, max_))
-        self.ids.sweep_center.setValue(center)
-        self.ids.sweep_amplitude.setValue(amplitude)
+        self.main_window.sweepSlider.blockSignals(True)
+        self.main_window.sweepAmplitudeSpinBox.blockSignals(True)
+        self.main_window.sweepCenterSpinBox.blockSignals(True)
+
+        self.main_window.sweepSlider.setValue((min_, max_))
+        self.main_window.sweepCenterSpinBox.setValue(center)
+        self.main_window.sweepAmplitudeSpinBox.setValue(amplitude)
         if self.parameters.sweep_pause.value:
-            self.ids.sweep_start_stop_button.setText("Start")
+            self.main_window.sweepStartStopPushButton.setText("Start")
         else:
-            self.ids.sweep_start_stop_button.setText("Pause")
+            self.main_window.sweepStartStopPushButton.setText("Pause")
 
-        self.ids.sweep_slider.blockSignals(False)
-        self.ids.sweep_center.blockSignals(False)
-        self.ids.sweep_amplitude.blockSignals(False)
+        self.main_window.sweepSlider.blockSignals(False)
+        self.main_window.sweepCenterSpinBox.blockSignals(False)
+        self.main_window.sweepAmplitudeSpinBox.blockSignals(False)
 
     def pause_or_resume_sweep(self):
         # If sweep is paused, resume it or vice versa.
         self.parameters.sweep_pause.value = not self.parameters.sweep_pause.value
         self.control.write_registers()
 
     def update_sweep_center(self, center):
@@ -90,16 +99,16 @@
         amplitude = (max_ - min_) / 2
         center = (max_ + min_) / 2
         self.parameters.sweep_amplitude.value = amplitude
         self.parameters.sweep_center.value = center
         self.control.write_registers()
 
 
-class SweepSlider(superqt.QDoubleRangeSlider, CustomWidget):
+class SweepSlider(superqt.QDoubleRangeSlider):
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super(SweepSlider, self).__init__(*args, **kwargs)
 
-    def init(self):
+    def ready(self):
         # set control boundaries
         self.setMinimum(-1.0)
         self.setMaximum(1.0)
         self.setSingleStep(0.001)
```

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/version_checker.py` & `linien-gui-0.8.0rc1/linien_gui/ui/version_checker.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.7.0rc2/linien_gui/ui/view_panel.ui` & `linien-gui-0.8.0rc1/linien_gui/ui/view_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.7.0rc2/linien_gui/utils.py` & `linien-gui-0.8.0rc1/linien_gui/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,28 +13,42 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
+from typing import TYPE_CHECKING, Any, Callable
 
+from linien_client.remote_parameters import RemoteParameter
+from PyQt5 import QtWidgets
 from PyQt5.QtWidgets import (
     QCheckBox,
     QComboBox,
     QDoubleSpinBox,
     QRadioButton,
     QSlider,
     QSpinBox,
     QTabWidget,
 )
 from pyqtgraph.Qt import QtGui
 
+if TYPE_CHECKING:
+    from linien_gui.app import LinienApp
 
-def param2ui(parameter, element, process_value=lambda x: x):
+
+def get_linien_app_instance() -> "LinienApp":
+    return QtWidgets.QApplication.instance()  # type: ignore[return-value]
+
+
+def param2ui(
+    parameter: RemoteParameter,
+    element: QtWidgets.QTabWidget,
+    process_value: Callable[[Any], Any] = lambda x: x,
+):
     """
     Updates ui elements according to parameter values.
 
     Listens to parameter changes and sets the value of `element` automatically.
     Optionally, the value can be processed using `process_value`. This function should
     be used because it automatically blocks signal emission from the target element;
     otherwise this can cause nasty endless loops when quickly changing a paramater
@@ -53,15 +67,15 @@
         elif isinstance(element, (QTabWidget, QComboBox)):
             element.setCurrentIndex(int(value))
         else:
             raise TypeError(f"Unsupported element type {type(element)}")
 
         element.blockSignals(False)
 
-    parameter.on_change(on_change)
+    parameter.add_callback(on_change)
 
 
 def set_window_icon(window):
     icon_name = os.path.join(*os.path.split(__file__)[:-1], "icon.ico")
     window.setWindowIcon(QtGui.QIcon(icon_name))
```

### Comparing `linien-gui-0.7.0rc2/linien_gui.egg-info/PKG-INFO` & `linien-gui-0.8.0rc1/linien_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 0.7.0rc2
+Version: 0.8.0rc1
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-gui-0.7.0rc2/linien_gui.egg-info/SOURCES.txt` & `linien-gui-0.8.0rc1/linien_gui.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 linien_gui/ui/device_manager.py
 linien_gui/ui/device_manager.ui
 linien_gui/ui/general_panel.py
 linien_gui/ui/general_panel.ui
 linien_gui/ui/lock_status_panel.py
 linien_gui/ui/locking_panel.py
 linien_gui/ui/locking_panel.ui
+linien_gui/ui/logging_panel.py
+linien_gui/ui/logging_panel.ui
 linien_gui/ui/main_window.py
 linien_gui/ui/main_window.ui
 linien_gui/ui/modulation_sweep_panel.py
 linien_gui/ui/modulation_sweep_panel.ui
 linien_gui/ui/new_device_dialog.py
 linien_gui/ui/new_device_dialog.ui
 linien_gui/ui/optimization_panel.py
```

### Comparing `linien-gui-0.7.0rc2/setup.py` & `linien-gui-0.8.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "0.7.0rc2"
+version = "0.8.0rc1"
 
 setup(
     name="linien-gui",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
@@ -36,15 +36,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     entry_points={"console_scripts": ["linien=linien_gui.app:run_application"]},
     python_requires=">=3.8",
     install_requires=[
-        "appdirs>=1.4.4",
+        "app_paths>=0.0.7 ",
         "click>=7.1.2",
         "pyqtgraph>=0.10.0",
         "PyQt5>=5.12.0",
         "superqt>=0.2.3",
         f"linien_client=={version}",
     ],
     package_data={
```

