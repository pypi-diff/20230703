# Comparing `tmp/q2gui-0.1.96.tar.gz` & `tmp/q2gui-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2gui-0.1.96.tar", max compression
+gzip compressed data, was "q2gui-0.1.97.tar", max compression
```

## Comparing `q2gui-0.1.96.tar` & `q2gui-0.1.97.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2gui-0.1.96/LICENSE
--rw-r--r--   0        0        0      576 2023-07-01 16:40:21.538590 q2gui-0.1.96/pyproject.toml
--rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.96/q2gui/__init__.py
--rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.96/q2gui/__main__.py
--rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.96/q2gui/pyqt6/__init__.py
--rw-r--r--   0        0        0    18937 2023-07-01 11:48:44.092567 q2gui-0.1.96/q2gui/pyqt6/q2app.py
--rw-r--r--   0        0        0    10075 2023-06-25 14:11:17.663886 q2gui-0.1.96/q2gui/pyqt6/q2form.py
--rw-r--r--   0        0        0      934 2023-06-25 14:11:34.825464 q2gui-0.1.96/q2gui/pyqt6/q2model.py
--rw-r--r--   0        0        0    10507 2023-06-28 19:48:59.612135 q2gui-0.1.96/q2gui/pyqt6/q2style.py
--rw-r--r--   0        0        0     8704 2023-06-30 09:15:23.522377 q2gui-0.1.96/q2gui/pyqt6/q2widget.py
--rw-r--r--   0        0        0     4982 2023-06-29 15:09:52.465129 q2gui-0.1.96/q2gui/pyqt6/q2window.py
--rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.96/q2gui/pyqt6/widgets/__init__.py
--rw-r--r--   0        0        0     1945 2023-06-25 14:12:17.787215 q2gui-0.1.96/q2gui/pyqt6/widgets/q2button.py
--rw-r--r--   0        0        0     2604 2023-06-25 14:12:24.675295 q2gui-0.1.96/q2gui/pyqt6/widgets/q2check.py
--rw-r--r--   0        0        0    16742 2023-06-28 20:23:31.010565 q2gui-0.1.96/q2gui/pyqt6/widgets/q2code.py
--rw-r--r--   0        0        0     1997 2023-06-25 14:14:55.047159 q2gui-0.1.96/q2gui/pyqt6/widgets/q2combo.py
--rw-r--r--   0        0        0     7052 2023-06-30 09:30:48.477542 q2gui-0.1.96/q2gui/pyqt6/widgets/q2date.py
--rw-r--r--   0        0        0     1423 2023-06-30 09:29:17.097202 q2gui-0.1.96/q2gui/pyqt6/widgets/q2doublespin.py
--rw-r--r--   0        0        0     3996 2023-06-25 14:14:16.859234 q2gui-0.1.96/q2gui/pyqt6/widgets/q2frame.py
--rw-r--r--   0        0        0     9350 2023-06-28 18:27:25.949985 q2gui-0.1.96/q2gui/pyqt6/widgets/q2grid.py
--rw-r--r--   0        0        0     4910 2023-06-25 14:15:06.706273 q2gui-0.1.96/q2gui/pyqt6/widgets/q2image.py
--rw-r--r--   0        0        0     2326 2023-06-30 09:16:34.186384 q2gui-0.1.96/q2gui/pyqt6/widgets/q2label.py
--rw-r--r--   0        0        0     4990 2023-06-25 14:13:01.287625 q2gui-0.1.96/q2gui/pyqt6/widgets/q2line.py
--rw-r--r--   0        0        0     1832 2023-06-25 14:13:04.950023 q2gui-0.1.96/q2gui/pyqt6/widgets/q2list.py
--rw-r--r--   0        0        0     3400 2023-06-25 14:13:08.964479 q2gui-0.1.96/q2gui/pyqt6/widgets/q2lookup.py
--rw-r--r--   0        0        0     1288 2023-06-25 14:13:12.427853 q2gui-0.1.96/q2gui/pyqt6/widgets/q2progressbar.py
--rw-r--r--   0        0        0     3002 2023-06-25 14:14:45.832847 q2gui-0.1.96/q2gui/pyqt6/widgets/q2radio.py
--rw-r--r--   0        0        0     7206 2023-06-25 14:13:35.252403 q2gui-0.1.96/q2gui/pyqt6/widgets/q2relation.py
--rw-r--r--   0        0        0      998 2023-06-25 14:15:42.427890 q2gui-0.1.96/q2gui/pyqt6/widgets/q2scroller.py
--rw-r--r--   0        0        0    17399 2023-06-25 14:15:37.873742 q2gui-0.1.96/q2gui/pyqt6/widgets/q2sheet.py
--rw-r--r--   0        0        0     1118 2023-07-01 10:11:15.099025 q2gui-0.1.96/q2gui/pyqt6/widgets/q2space.py
--rw-r--r--   0        0        0     1232 2023-06-30 09:29:03.480058 q2gui-0.1.96/q2gui/pyqt6/widgets/q2spin.py
--rw-r--r--   0        0        0     3934 2023-07-01 14:42:37.242752 q2gui-0.1.96/q2gui/pyqt6/widgets/q2tab.py
--rw-r--r--   0        0        0     1545 2023-06-25 14:15:20.976634 q2gui-0.1.96/q2gui/pyqt6/widgets/q2text.py
--rw-r--r--   0        0        0     7538 2023-06-25 14:15:16.690766 q2gui-0.1.96/q2gui/pyqt6/widgets/q2toolbar.py
--rw-r--r--   0        0        0     1168 2023-06-30 09:23:45.362000 q2gui-0.1.96/q2gui/pyqt6/widgets/q2toolbutton.py
--rw-r--r--   0        0        0    21326 2023-06-30 13:00:29.804624 q2gui-0.1.96/q2gui/q2app.py
--rw-r--r--   0        0        0    12944 2023-06-29 20:34:11.352834 q2gui-0.1.96/q2gui/q2dialogs.py
--rw-r--r--   0        0        0    69652 2023-07-01 09:42:25.792695 q2gui-0.1.96/q2gui/q2form.py
--rw-r--r--   0        0        0    15709 2023-06-25 14:10:22.631445 q2gui-0.1.96/q2gui/q2model.py
--rw-r--r--   0        0        0     5909 2023-06-25 14:10:31.421051 q2gui-0.1.96/q2gui/q2style.py
--rw-r--r--   0        0        0     1513 2023-06-25 14:11:23.976312 q2gui-0.1.96/q2gui/q2utils.py
--rw-r--r--   0        0        0     5945 2023-07-01 10:59:16.641839 q2gui-0.1.96/q2gui/q2widget.py
--rw-r--r--   0        0        0     3814 2023-06-25 14:10:50.574661 q2gui-0.1.96/q2gui/q2window.py
--rw-r--r--   0        0        0       22 2023-07-01 16:40:24.733400 q2gui-0.1.96/q2gui/version.py
--rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.96/README.md
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.96/PKG-INFO
+-rw-r--r--   0        0        0    10347 2023-06-21 10:29:20.277459 q2gui-0.1.97/LICENSE
+-rw-r--r--   0        0        0      576 2023-07-02 23:22:55.519543 q2gui-0.1.97/pyproject.toml
+-rw-r--r--   0        0        0       39 2022-12-11 17:39:14.961644 q2gui-0.1.97/q2gui/__init__.py
+-rw-r--r--   0        0        0      892 2022-12-11 17:39:14.961644 q2gui-0.1.97/q2gui/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-11 17:39:14.961644 q2gui-0.1.97/q2gui/pyqt6/__init__.py
+-rw-r--r--   0        0        0    22910 2023-07-02 20:43:43.643405 q2gui-0.1.97/q2gui/pyqt6/q2app.py
+-rw-r--r--   0        0        0    10075 2023-06-25 14:11:17.663886 q2gui-0.1.97/q2gui/pyqt6/q2form.py
+-rw-r--r--   0        0        0      934 2023-06-25 14:11:34.825464 q2gui-0.1.97/q2gui/pyqt6/q2model.py
+-rw-r--r--   0        0        0    10507 2023-06-28 19:48:59.612135 q2gui-0.1.97/q2gui/pyqt6/q2style.py
+-rw-r--r--   0        0        0     8704 2023-06-30 09:15:23.522377 q2gui-0.1.97/q2gui/pyqt6/q2widget.py
+-rw-r--r--   0        0        0     4982 2023-06-29 15:09:52.465129 q2gui-0.1.97/q2gui/pyqt6/q2window.py
+-rw-r--r--   0        0        0      754 2023-02-06 11:50:26.449600 q2gui-0.1.97/q2gui/pyqt6/widgets/__init__.py
+-rw-r--r--   0        0        0     1945 2023-06-25 14:12:17.787215 q2gui-0.1.97/q2gui/pyqt6/widgets/q2button.py
+-rw-r--r--   0        0        0     2604 2023-06-25 14:12:24.675295 q2gui-0.1.97/q2gui/pyqt6/widgets/q2check.py
+-rw-r--r--   0        0        0    16742 2023-06-28 20:23:31.010565 q2gui-0.1.97/q2gui/pyqt6/widgets/q2code.py
+-rw-r--r--   0        0        0     1997 2023-06-25 14:14:55.047159 q2gui-0.1.97/q2gui/pyqt6/widgets/q2combo.py
+-rw-r--r--   0        0        0     7052 2023-06-30 09:30:48.477542 q2gui-0.1.97/q2gui/pyqt6/widgets/q2date.py
+-rw-r--r--   0        0        0     1423 2023-06-30 09:29:17.097202 q2gui-0.1.97/q2gui/pyqt6/widgets/q2doublespin.py
+-rw-r--r--   0        0        0     3996 2023-06-25 14:14:16.859234 q2gui-0.1.97/q2gui/pyqt6/widgets/q2frame.py
+-rw-r--r--   0        0        0     9350 2023-06-28 18:27:25.949985 q2gui-0.1.97/q2gui/pyqt6/widgets/q2grid.py
+-rw-r--r--   0        0        0     4910 2023-06-25 14:15:06.706273 q2gui-0.1.97/q2gui/pyqt6/widgets/q2image.py
+-rw-r--r--   0        0        0     2326 2023-06-30 09:16:34.186384 q2gui-0.1.97/q2gui/pyqt6/widgets/q2label.py
+-rw-r--r--   0        0        0     4990 2023-06-25 14:13:01.287625 q2gui-0.1.97/q2gui/pyqt6/widgets/q2line.py
+-rw-r--r--   0        0        0     1832 2023-06-25 14:13:04.950023 q2gui-0.1.97/q2gui/pyqt6/widgets/q2list.py
+-rw-r--r--   0        0        0     3400 2023-06-25 14:13:08.964479 q2gui-0.1.97/q2gui/pyqt6/widgets/q2lookup.py
+-rw-r--r--   0        0        0     1288 2023-06-25 14:13:12.427853 q2gui-0.1.97/q2gui/pyqt6/widgets/q2progressbar.py
+-rw-r--r--   0        0        0     3002 2023-06-25 14:14:45.832847 q2gui-0.1.97/q2gui/pyqt6/widgets/q2radio.py
+-rw-r--r--   0        0        0     7206 2023-06-25 14:13:35.252403 q2gui-0.1.97/q2gui/pyqt6/widgets/q2relation.py
+-rw-r--r--   0        0        0      998 2023-06-25 14:15:42.427890 q2gui-0.1.97/q2gui/pyqt6/widgets/q2scroller.py
+-rw-r--r--   0        0        0    17399 2023-06-25 14:15:37.873742 q2gui-0.1.97/q2gui/pyqt6/widgets/q2sheet.py
+-rw-r--r--   0        0        0     1118 2023-07-01 10:11:15.099025 q2gui-0.1.97/q2gui/pyqt6/widgets/q2space.py
+-rw-r--r--   0        0        0     1232 2023-06-30 09:29:03.480058 q2gui-0.1.97/q2gui/pyqt6/widgets/q2spin.py
+-rw-r--r--   0        0        0     3934 2023-07-01 14:42:37.242752 q2gui-0.1.97/q2gui/pyqt6/widgets/q2tab.py
+-rw-r--r--   0        0        0     1545 2023-06-25 14:15:20.976634 q2gui-0.1.97/q2gui/pyqt6/widgets/q2text.py
+-rw-r--r--   0        0        0     7538 2023-06-25 14:15:16.690766 q2gui-0.1.97/q2gui/pyqt6/widgets/q2toolbar.py
+-rw-r--r--   0        0        0     1168 2023-06-30 09:23:45.362000 q2gui-0.1.97/q2gui/pyqt6/widgets/q2toolbutton.py
+-rw-r--r--   0        0        0    21326 2023-06-30 13:00:29.804624 q2gui-0.1.97/q2gui/q2app.py
+-rw-r--r--   0        0        0    12944 2023-07-02 22:59:21.715306 q2gui-0.1.97/q2gui/q2dialogs.py
+-rw-r--r--   0        0        0    69700 2023-07-02 23:00:51.480140 q2gui-0.1.97/q2gui/q2form.py
+-rw-r--r--   0        0        0    15855 2023-07-02 15:02:12.981402 q2gui-0.1.97/q2gui/q2model.py
+-rw-r--r--   0        0        0     5909 2023-06-25 14:10:31.421051 q2gui-0.1.97/q2gui/q2style.py
+-rw-r--r--   0        0        0     1513 2023-06-25 14:11:23.976312 q2gui-0.1.97/q2gui/q2utils.py
+-rw-r--r--   0        0        0     5945 2023-07-01 10:59:16.641839 q2gui-0.1.97/q2gui/q2widget.py
+-rw-r--r--   0        0        0     3814 2023-06-25 14:10:50.574661 q2gui-0.1.97/q2gui/q2window.py
+-rw-r--r--   0        0        0       22 2023-07-02 23:23:00.353459 q2gui-0.1.97/q2gui/version.py
+-rw-r--r--   0        0        0     1533 2022-12-11 17:39:14.929664 q2gui-0.1.97/README.md
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 q2gui-0.1.97/PKG-INFO
```

### Comparing `q2gui-0.1.96/LICENSE` & `q2gui-0.1.97/LICENSE`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/pyproject.toml` & `q2gui-0.1.97/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2gui"
-version = "0.1.96"
+version = "0.1.97"
 description = "Python GUI toolkit"
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1"
```

### Comparing `q2gui-0.1.96/q2gui/__main__.py` & `q2gui-0.1.97/q2gui/__main__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/q2app.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2code.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,517 +8,425 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+import sys
+
 if __name__ == "__main__":
-    import sys
 
     sys.path.insert(0, ".")
 
     from demo.demo import demo
 
     demo()
 
-
-# from q2gui import q2form
-
-import os
-
+# from PyQt6.QtWidgets import QTextEdit, QSizePolicy
 from PyQt6.QtWidgets import (
-    QApplication,
+    QVBoxLayout,
+    QHBoxLayout,
     QWidget,
-    QMainWindow,
-    QToolButton,
-    QTextEdit,
-    QToolBar,
-    QFileDialog,
-    QTabWidget,
-    QTabBar,
-    QSplitter,
-    QMdiArea,
 )
 
-from PyQt6.QtCore import QEvent, Qt, QCoreApplication, QTimer
-from PyQt6.QtGui import QFontMetrics, QIcon, QFont, QBrush, QColor, QShortcut, QKeySequence
+from PyQt6.Qsci import QsciScintilla, QsciLexerPython, QsciLexerSQL, QsciLexerJSON, QsciAPIs, QsciLexer
+from PyQt6.QtGui import QColor
 
-from q2gui.pyqt6.q2window import Q2QtWindow
-from q2gui.pyqt6.q2style import Q2Style
-from q2gui.pyqt6.widgets.q2frame import q2frame
-from q2gui.pyqt6.widgets.q2space import q2space
-from q2gui.pyqt6.widgets.q2toolbutton import q2toolbutton
-
-
-import q2gui.q2app as q2app
-
-
-class stdout_widget(q2frame):
-    def __init__(self, mode="h"):
-        super().__init__({"column": "/h", "label": "Output"})
-        self.stdout_widget = QTextEdit(self)
-
-        self.toolbar_frame = q2frame({"column": "/v"})
-        self.closeButton = q2toolbutton(self.make_meta(column="hide", label="❌", mess="Hide output"))
-        self.closeButton.clicked.connect(lambda: self.hide())
-
-        self.cleanButton = q2toolbutton(self.make_meta(label="🧹", mess="Clean output"))
-        self.cleanButton.clicked.connect(self.stdout_widget.clear)
-
-        self.toolbar_frame.insert_widget(widget=self.closeButton)
-        # self.toolbar_frame.insert_widget(widget=q2space())
-        self.toolbar_frame.insert_widget(widget=self.cleanButton)
-
-        self.insert_widget(widget=self.stdout_widget)
-        self.insert_widget(widget=self.toolbar_frame)
-        self.setVisible(False)
-
-    def write(self, text):
-        if not self.isVisible():
-            self.setVisible(True)
-        from PyQt6.QtGui import QTextCursor
-
-        self.stdout_widget.moveCursor(QTextCursor.MoveOperation.End)
-        q2app.q2_app.process_events()
-        self.stdout_widget.insertPlainText(text)
-
-
-class Q2App(QMainWindow, q2app.Q2App, Q2QtWindow):
-    class Q2TabWidget(QTabWidget):
-        def __init__(self, parent):
-            super().__init__(parent)
-            self.main_window: Q2App = parent
-            self.addTab(QWidget(), "+")
-            self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
-            self.setObjectName("main_tab_widget")
-            self.prev_index = None
-            self.tab_focus_widget = {}
-            self.tabBar().setObjectName("main_tab_bar")
-
-            self.closeButton = QToolButton(self)
-            self.closeButton.setText("❌")
-            self.closeButton.clicked.connect(self.closeSubWindow)
-            self.setCornerWidget(self.closeButton)
-            self.currentChanged.connect(self.restore_tab_focus_widget)
-
-        def hide(self) -> None:
-            self.tabBar().hide()
-            self.closeButton.hide()
-            # return super().hide()
-
-        def show(self) -> None:
-            self.tabBar().show()
-            self.closeButton.show()
-            # return super().show()
-
-        def save_tab_focus_widget(self, widget):
-            self.tab_focus_widget[self.currentIndex()] = widget
-
-        def restore_tab_focus_widget(self):
-            if self.currentIndex() == self.count() - 1:
-                self.addTab()
-                return
-            focus_widget = self.tab_focus_widget.get(self.currentIndex(), self)
-            if focus_widget:
-                try:
-                    focus_widget.setFocus()
-                except Exception:
-                    pass
-
-        def closeSubWindow(self):
-            currentTabIndex = self.currentIndex()
-            if self.currentWidget().activeSubWindow():
-                self.currentWidget().activeSubWindow().close()
-            elif self.count() > 2:  # close tab if them >2
-                self.setCurrentIndex(currentTabIndex - 1)
-                self.removeTab(currentTabIndex)
-
-        def addTab(self, widget=None, label="="):
-            if not widget:
-                widget = QMdiArea(self)
-                self.set_tab_background(widget)
-                widget.form_level = 0
-                widget.setOption(QMdiArea.AreaOption.DontMaximizeSubWindowOnActivation)
-                widget.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAsNeeded)
-                widget.setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAsNeeded)
-
-            self.insertTab(self.count() - 1, widget, label)
-            self.setCurrentIndex(self.count() - 2)
-            if self.count() > 1:
-                self.main_window.on_new_tab()
-
-        def set_tab_background(self, widget):
-            if isinstance(widget, QMdiArea):
-                if self.main_window.q2style.color_mode == "clean":
-                    widget.setBackground(QBrush(QApplication.palette().dark()))
-                else:
-                    widget.setBackground(
-                        QBrush(QColor(self.main_window.q2style.get_style("background_disabled")))
-                    )
-
-        def set_tabs_backround(self):
-            for x in range(self.count()):
-                self.set_tab_background(self.widget(x))
-
-    def __init__(self, title=""):
-        if QCoreApplication.startingUp():  # one and only QApplication allowed
-            self.QApplication = QApplication([])
-        QMainWindow.__init__(self)
-        Q2QtWindow.__init__(self)
-        self.q2_tabwidget = self.Q2TabWidget(self)
-        self.q2_toolbar = QToolBar(self)
-        self.stdout_widget = stdout_widget()
-
-        self.Q2Style = Q2Style
-        q2app.Q2App.__init__(self)
-
-        if not hasattr(QApplication, "_mw_count"):
-            QApplication._mw_count = 0
-            QApplication._mw_list = []
-        QApplication._mw_count += 1
-        QApplication._mw_list.append(self)
-        self.closing = False
-
-        self.central_widget = QSplitter(Qt.Orientation.Vertical)
-        self.setCentralWidget(self.central_widget)
-        self.centralWidget().setObjectName("central_widget")
-
-        self.addToolBar(self.q2_toolbar)
-
-        self.central_widget.addWidget(self.q2_tabwidget)
-        self.central_widget.addWidget(self.stdout_widget)
-        self.central_widget.setSizes(
-            [
-                10,
-            ]
-        )
-
-        self.statusBar().setVisible(True)
-        self.set_title(title)
+# from PyQt6.QtWidgets import QMenu
+from PyQt6.QtCore import Qt, QTimer, QSize
 
-        QApplication.instance().focusChanged.connect(self.focus_changed)
-        QApplication.instance().focusChanged.connect(self.save_tab_focus_widget)
-
-        self.next_tab_shortcut = QShortcut(QKeySequence("Ctrl+Tab"), self)
-        self.prev_tab_shortcut = QShortcut(QKeySequence("Ctrl+Shift+Tab"), self)
-        self.next_tab_shortcut.activated.connect(
-            lambda: self.q2_tabwidget.setCurrentIndex(self.q2_tabwidget.currentIndex() + 1)
-            if self.q2_tabwidget.tabBar().isVisible()
-            else None
-        )
-        self.prev_tab_shortcut.activated.connect(
-            lambda: self.q2_tabwidget.setCurrentIndex(self.q2_tabwidget.currentIndex() - 1)
-            if self.q2_tabwidget.tabBar().isVisible()
-            else None
-        )
-
-        # replace static methods for instance
-        self.get_open_file_dialoq = self._get_open_file_dialoq
-        self.get_save_file_dialoq = self._get_save_file_dialoq
-        self._last_get_file_path = None
-
-    def set_font(self, font_name="", font_size=12):
-        QApplication.setFont(QFont(font_name, font_size))
-
-    def save_tab_focus_widget(self):
-        self.q2_tabwidget.save_tab_focus_widget(self.focus_widget())
-
-    def get_self(self):
-        if QApplication.activeWindow():
-            return QApplication.activeWindow()
-        else:
-            return self
-
-    def eventFilter(self, obj, ev: QEvent):
-        if ev.type() == QEvent.Type.Close:
-            if obj.heap.prev_mdi_window:
-                obj.heap.prev_mdi_window.setEnabled(True)
-
-            if obj.heap.prev_focus_widget is not None and not isinstance(obj.heap.prev_focus_widget, QTabBar):
-                # print(obj.heap.prev_focus_widget)
-                try:
-                    obj.heap.prev_focus_widget.setFocus()
-                except Exception:
-                    pass
-            self.set_tabbar_text(obj.heap.prev_tabbar_text)
-            if obj.heap.modal == "super":  # real modal dialog
-                self.disable_toolbar(False)
-                self.disable_menubar(False)
-                self.disable_tabbar(False)
-
-        return super().eventFilter(obj, ev)
-
-    def show_form(self, form=None, modal="modal"):
-        form.heap = q2app.Q2Heap()
-        form.heap.modal = modal
-        form.heap.prev_mdi_window = self.q2_tabwidget.currentWidget().activeSubWindow()
-        form.heap.prev_focus_widget = QApplication.focusWidget()
-        form.heap.prev_tabbar_text = self.get_tabbar_text()
-
-        self.q2_tabwidget.currentWidget().addSubWindow(form)
-        form.installEventFilter(self)
-
-        if modal != "" and form.heap.prev_mdi_window:  # mdiarea normal window
-            form.heap.prev_mdi_window.setDisabled(True)
-
-        self.set_tabbar_text(form.window_title)
-
-        if modal == "super":  # real modal dialog
-            self.disable_toolbar(True)
-            self.disable_menubar(True)
-            self.disable_tabbar(True)
-        if modal == "":  # mdiarea normal window
-            form.show()
+from q2gui.pyqt6.q2widget import Q2Widget
+from q2gui.pyqt6.widgets.q2line import q2line
+from q2gui.pyqt6.widgets.q2label import q2label
+from q2gui.pyqt6.widgets.q2button import q2button
+from q2gui.q2utils import int_
+
+
+class q2code(QsciScintilla, Q2Widget):
+    def __init__(self, meta):
+        super().__init__(meta)
+        self.setUtf8(True)
+        self.setFolding(QsciScintilla.FoldStyle.BoxedTreeFoldStyle)
+
+        self.lexer: QsciLexer = None
+        self.set_lexer()
+        self.set_background_color()
+
+        self.setAutoIndent(True)
+        self.setIndentationGuides(True)
+        self.setIndentationsUseTabs(False)
+        self.setBraceMatching(QsciScintilla.BraceMatch.StrictBraceMatch)
+        self.setMarginLineNumbers(1, True)
+        self.setMarginWidth(1, "9999")
+        self.setTabWidth(4)
+
+        self.setAutoCompletionSource(QsciScintilla.AutoCompletionSource.AcsAll)
+        self.setAutoCompletionCaseSensitivity(True)
+        self.setAutoCompletionReplaceWord(True)
+        self.setAutoCompletionThreshold(1)
+
+        self.SCN_DOUBLECLICK
+
+        self.setCaretLineVisible(True)
+
+        self.searchIndicator = QsciScintilla.INDIC_CONTAINER
+        self.SendScintilla(QsciScintilla.SCI_INDICSETSTYLE, self.searchIndicator, QsciScintilla.INDIC_BOX)
+        self.SendScintilla(QsciScintilla.SCI_INDICSETFORE, self.searchIndicator, QColor("red"))
+
+        self.cursorPositionChanged.connect(self.__cursorPositionChanged)
+        self.__markOccurrencesTimer = QTimer(self)
+        self.__markOccurrencesTimer.setSingleShot(True)
+        self.__markOccurrencesTimer.setInterval(500)
+        self.__markOccurrencesTimer.timeout.connect(self.__markOccurrences)
+        self.textChanged.connect(self.valid)
+        # self.setContextMenuPolicy(Qt.ContextMenuPolicy.ActionsContextMenu)
+        self.editor_panel = q2editor_panel(self)
+        self.create_context_menu()
+        self.set_custom_autocompletition_list()
+
+    def set_lexer(self, lexer=""):
+        if lexer == "":
+            lexer = self.meta["control"]
+        if "python" in lexer:
+            self.lexer = QsciLexerPython()
+        elif "sql" in lexer:
+            self.lexer = QsciLexerSQL()
+        elif "json" in lexer:
+            self.lexer = QsciLexerJSON()
         else:
-            form.exec()
+            self.lexer = QsciLexerPython()
+        if self.lexer:
+            self.setLexer(self.lexer)
+
+    def set_custom_autocompletition_list(self, custom_autocompletions_list=[]):
+        custom_autocompletions_list = self.meta["form"].q2_app.get_autocompletition_list()
+        self.__api = QsciAPIs(self.lexer)
+        for ac in custom_autocompletions_list:
+            self.__api.add(ac)
+        self.__api.prepare()
+
+    def set_background_color(self, red=150, green=200, blue=230):
+        # color_mode = self.meta.get("q2_app").q2style.get_system_color_mode()
+        # print(color_mode, self.meta.get("q2_app").q2style.color_mode)
+        # b_color = QColor(self.meta.get("q2_app").q2style.styles.get(color_mode).get("background"))
+        # f_color = QColor(self.meta.get("q2_app").q2style.styles.get(color_mode).get("color"))
+
+        # self.setMatchedBraceForegroundColor(QColor("lightgreen"))
+        self.lexer.setDefaultPaper(QColor(red, green, blue))
+        self.lexer.setPaper(QColor(red, green, blue))
+        # self.lexer.setDefaultPaper(b_color)
+        # self.lexer.setPaper(b_color)
+        # self.lexer.setColor(f_color, 5)
+        self.setMarginsForegroundColor(QColor("black"))
+        self.setMarginsBackgroundColor(QColor("gray"))
+
+    def __cursorPositionChanged(self, line, index):
+        self.__markOccurrencesTimer.stop()
+        self.clearIndicatorRange(
+            0, 0, self.lines() - 1, len(self.text(self.lines() - 1)), self.searchIndicator
+        )
+        self.__markOccurrencesTimer.start()
 
-    def disable_current_form(self, mode=True):
-        if self.q2_tabwidget.currentWidget().subWindowList():
-            prev_mdi_window = self.q2_tabwidget.currentWidget().subWindowList()[-1]
-            if prev_mdi_window:
-                prev_mdi_window.setDisabled(mode)
-                prev_mdi_window.setFocus()
-
-    def build_menu(self):
-        self.menu_list = super().reorder_menu(self.menu_list)
-        self._main_menu = {}
-        QMainWindow.menuBar(self).clear()
-        self.q2_toolbar.clear()
-        QMainWindow.menuBar(self).show()
-        for x in self.menu_list:
-            _path = x["TEXT"]
-            if _path == "" or _path in self._main_menu:
-                continue
-            prevNode = "|".join(_path.split("|")[:-1])
-            topic = _path.split("|")[-1]
-            if _path.count("|") == 0:  # first in chain - menu bar
-                node = QMainWindow.menuBar(self)
+    def __findFirstTarget(self, text):
+        if text == "":
+            return False
+        self.__targetSearchExpr = text.encode("utf-8")
+        self.__targetSearchFlags = QsciScintilla.SCFIND_MATCHCASE | QsciScintilla.SCFIND_WHOLEWORD
+        self.__targetSearchStart = 0
+        self.__targetSearchEnd = self.SendScintilla(QsciScintilla.SCI_GETTEXTLENGTH)
+        self.__targetSearchActive = True
+        return self.__doSearchTarget()
+
+    def __findNextTarget(self):
+        if not self.__targetSearchActive:
+            return False
+        return self.__doSearchTarget()
+
+    def __doSearchTarget(self):
+        if self.__targetSearchStart == self.__targetSearchEnd:
+            self.__targetSearchActive = False
+            return False
+        self.SendScintilla(QsciScintilla.SCI_SETTARGETSTART, self.__targetSearchStart)
+        self.SendScintilla(QsciScintilla.SCI_SETTARGETEND, self.__targetSearchEnd)
+        self.SendScintilla(QsciScintilla.SCI_SETSEARCHFLAGS, self.__targetSearchFlags)
+        pos = self.SendScintilla(
+            QsciScintilla.SCI_SEARCHINTARGET, len(self.__targetSearchExpr), self.__targetSearchExpr
+        )
+        if pos == -1:
+            self.__targetSearchActive = False
+            return False
+        self.SendScintilla(QsciScintilla.SCI_INDICATORFILLRANGE, pos, len(self.__targetSearchExpr))
+        targend = self.SendScintilla(QsciScintilla.SCI_GETTARGETEND)
+        self.__targetSearchStart = targend
+        return True
+
+    def __markOccurrences(self):
+        if self.hasFocus():
+            line, index = self.getCursorPosition()
+            ok = self.__findFirstTarget(self.__getWord(self.text(line), index - 1))
+            while ok:
+                ok = self.__findNextTarget()
+
+    def __getWord(self, text, index):
+        word = ""
+        for x in range(index, -1, -1):
+            if text[x].isalpha() or text[x].isdigit():
+                word = text[x] + word
             else:
-                node = self._main_menu.get(prevNode)
-                if node is None:
-                    node = QMainWindow.menuBar(self)
-            if _path.endswith("-"):
-                node.addSeparator()
-            elif x["WORKER"]:
-                self._main_menu[_path] = node.addAction(topic)
-                self._main_menu[_path].triggered.connect(x["WORKER"])
-
-                icon = self.get_icon(x["ICON"])
-                if icon:
-                    self._main_menu[_path].setIcon(QIcon(icon))
-
-                if x["TOOLBAR"]:
-                    button = QToolButton(self)
-                    button.setText(topic)
-                    button.setDefaultAction(self._main_menu[_path])
-                    self.q2_toolbar.addAction(self._main_menu[_path])
+                break
+        for x in range(index + 1, len(text)):
+            if text[x].isalpha() or text[x].isdigit():
+                word += text[x]
             else:
-                self._main_menu[_path] = node.addMenu(topic)
-        # Show as context menu
-        self.setContextMenuPolicy(Qt.ContextMenuPolicy.ActionsContextMenu)
-        for a in self.actions():
-            self.removeAction(a)
-        self.addActions(self.menuBar().actions())
-
-    def set_color_mode(self, color_mode=None):
-        q2app.Q2App.set_color_mode(self, color_mode)
-        self.q2_tabwidget.set_tabs_backround()
-
-    def focus_widget(self):
-        return QApplication.focusWidget()
-
-    def get_clipboard_text(self):
-        return QApplication.clipboard().text()
-
-    def set_style_sheet(self, style=None):
-        if os.path.isfile(self.style_file):
-            try:
-                with open(self.style_file, "r") as style_data:
-                    local_style = style_data.read()
-            except Exception:
-                local_style = ""
-        else:
-            local_style = ""
-        self.setStyleSheet(style + local_style)
+                break
+        return word
 
-    def add_style_sheet(self, style):
-        current_style = self.styleSheet() + f"{style}"
-        self.setStyleSheet(current_style)
-
-    def lock(self):
-        self.menuBar().setDisabled(True)
-        self.q2_toolbar.setDisabled(True)
-        self.q2_tabwidget.setDisabled(True)
-
-    def unlock(self):
-        self.menuBar().setDisabled(False)
-        self.q2_toolbar.setDisabled(False)
-        self.q2_tabwidget.setDisabled(False)
-
-    def set_icon(self, icon_path):
-        self.icon = icon_path
-        self.setWindowIcon(QIcon(self.icon))
-
-    def process_events(self):
-        QApplication.processEvents()
-
-    def show_menubar(self, mode=True):
-        q2app.Q2App.show_menubar(self)
-        if mode:
-            QMainWindow.menuBar(self).show()
-        else:
-            QMainWindow.menuBar(self).hide()
+    def mouseDoubleClickEvent(self, event):
+        return super().mouseDoubleClickEvent(event)
 
-    def is_menubar_visible(self):
-        return QMainWindow.menuBar(self).isVisible()
+    def create_context_menu(self):
+        self.context_menu = self.createStandardContextMenu()
+        self.context_menu.addSeparator()
+
+        find_action = self.context_menu.addAction("Find")
+        find_action.triggered.connect(self.editor_panel.show_find)
+        find_action.setShortcuts(["Ctrl+F", "F3"])
+
+        replace_action = self.context_menu.addAction("Replace")
+        replace_action.triggered.connect(self.editor_panel.show_replace)
+        replace_action.setShortcut("Ctrl+H")
+
+        gotoline_action = self.context_menu.addAction("Go to line")
+        gotoline_action.triggered.connect(self.editor_panel.show_go)
+        gotoline_action.setShortcut("Ctrl+G")
+
+        self.context_menu.addSeparator()
+
+        fold_action = self.context_menu.addAction("Fold/Unfold")
+        fold_action.triggered.connect(self.perform_folding)
+        fold_action.setShortcuts(["Alt+Up", "Alt+Down"])
+
+        foldall_action = self.context_menu.addAction("Fold/Unfold All")
+        foldall_action.triggered.connect(self.foldAll)
+        foldall_action.setShortcuts(["Alt+Left", "Alt+Right"])
+
+        self.context_menu.addSeparator()
+        comment_action = self.context_menu.addAction("Comment/uncomment line(s)")
+        comment_action.setShortcut("Ctrl+3")
+        comment_action.triggered.connect(self.perform_comment)
+
+        complete_action = self.context_menu.addAction("Autocomplete")
+        complete_action.triggered.connect(self.autoCompleteFromAll)
+        complete_action.setShortcuts(["Ctrl+Space"])
+
+        self.addActions(self.context_menu.actions())
+        for x in self.context_menu.actions():
+            if x.isEnabled():
+                x.setVisible(True)
+            else:
+                x.setVisible(False)
 
-    def show_toolbar(self, mode=True):
-        q2app.Q2App.show_toolbar(self)
-        if mode:
-            self.q2_toolbar.show()
+    def perform_comment(self):
+        selected_lines = []
+        current_line, current_pos = self.getCursorPosition()
+        if self.hasSelectedText():
+            line1, pos1, line2, pos2 = self.getSelection()
+            for x in range(line1, line2 + 1):
+                selected_lines.append(x)
         else:
-            self.q2_toolbar.hide()
-
-    def disable_toolbar(self, mode=True):
-        self.q2_toolbar.setDisabled(True if mode else False)
-
-    def disable_menubar(self, mode=True):
-        QMainWindow.menuBar(self).setDisabled(True if mode else False)
+            selected_lines.append(current_line)
 
-    def disable_tabbar(self, mode=True):
-        self.q2_tabwidget.tabBar().setDisabled(True if mode else False)
-
-    def is_toolbar_visible(self):
-        return self.q2_toolbar.isVisible()
-
-    def show_tabbar(self, mode=True):
-        q2app.Q2App.show_tabbar(self)
-        if mode:
-            self.q2_tabwidget.show()
+        for line in selected_lines:
+            new_pos = self.comment_line(line, current_pos)
+            if line == current_line:
+                self.setCursorPosition(current_line, new_pos)
+
+        if len(selected_lines) > 1:
+            self.setSelection(line1, pos1, line2, pos2)
+
+    def comment_line(self, line, pos):
+        current_line = self.text(line)
+        if len(current_line.strip()):
+            if current_line.lstrip()[0:2] == "# ":
+                comment_pos = current_line.index("# ")
+                if comment_pos < pos:
+                    pos -= 2
+                self.setSelection(line, comment_pos, line, comment_pos + 2)
+                self.removeSelectedText()
+            else:
+                spaces_count = len(current_line) - len(current_line.lstrip())
+                if pos > spaces_count:
+                    pos += 2
+                self.insertAt("# ", line, spaces_count)
+        return pos
+
+    def perform_folding(self):
+        self.foldLine(self.getCursorPosition()[0])
+
+    def current_line(self):
+        return self.getCursorPosition()[0]
+
+    def goto_line(self, line=0):
+        self.setCursorPosition(int_(line) - 1, 0)
+        self.set_focus()
+        self.ensureLineVisible(self.getCursorPosition()[0])
+        self.editor_panel.close()
+
+    def contextMenuEvent(self, event):
+        self.create_context_menu()
+        self.context_menu.exec(event.globalPos())
+
+    def showEvent(self, ev):
+        self.updateGeometry()
+        return super().showEvent(ev)
+
+    def sizeHint(self):
+        if self.isVisible():
+            return QSize(99999, 99999)
         else:
-            self.q2_tabwidget.hide()
+            return super().sizeHint()
 
-    def is_tabbar_visible(self):
-        return self.q2_tabwidget.tabBar().isVisible()
 
-    def get_tabbar_text(self):
-        return self.q2_tabwidget.tabBar().tabText(self.q2_tabwidget.currentIndex())
-
-    def show_statusbar_mess(self, text=""):
-        self.statusBar().showMessage(f"{text}")
-
-    def set_tabbar_text(self, text=""):
-        self.q2_tabwidget.tabBar().setTabText(self.q2_tabwidget.currentIndex(), text)
-
-    def show_statusbar(self, mode=True):
-        q2app.Q2App.show_statusbar(self)
-        if mode:
-            self.statusBar().show()
+class q2editor_panel(QWidget):
+    def __init__(self, parent, text=""):
+        super().__init__(parent, Qt.WindowType.Popup)
+        # super().__init__(parent)
+        self.setLayout(QVBoxLayout())
+
+        self.layout().setContentsMargins(0, 0, 0, 0)
+        # self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
+        self.create_find()
+        self.create_replace()
+        self.create_go()
+
+        self.layout().addWidget(self.find_frame)
+        self.layout().addWidget(self.replace_frame)
+        self.layout().addWidget(self.go_frame)
+
+        self.set_find_text(text)
+        self.q2code: q2code = parent
+        self.last_find_direction = "down"
+
+    def create_find(self):
+        self.find_frame = QWidget()
+
+        self.find_frame.setLayout(QHBoxLayout())
+        self.find_frame.layout().setContentsMargins(0, 0, 0, 0)
+
+        self.find_next_button = q2button({"label": ">"})
+        self.find_next_button.set_fixed_width(3, "w")
+
+        self.find_prev_button = q2button({"label": "<"})
+        self.find_prev_button.set_fixed_width(3, "w")
+
+        self.find_text = q2line({})
+        self.find_frame.layout().addWidget(q2label({"label": "find:"}))
+        self.find_frame.layout().addWidget(self.find_text)
+        self.find_frame.layout().addWidget(self.find_prev_button)
+        self.find_frame.layout().addWidget(self.find_next_button)
+        self.find_next_button.pressed.connect(self.perform_find_next)
+        self.find_prev_button.pressed.connect(self.perform_find_prev)
+        self.find_text.keyPressEvent = self.find_keyPressEvent
+
+    def find_keyPressEvent(self, event):
+        if event.key() in [Qt.Key.Key_Up] or (
+            event.key() in [Qt.Key.Key_Enter, Qt.Key.Key_Return, Qt.Key.Key_F3]
+            and event.modifiers() == Qt.KeyboardModifier.ShiftModifier
+        ):
+            self.perform_find_prev()
+        elif event.key() in [Qt.Key.Key_Enter, Qt.Key.Key_Return, Qt.Key.Key_Down, Qt.Key.Key_F3]:
+            self.perform_find_next()
+        elif event.key() == Qt.Key.Key_H:
+            self.show_replace()
+        q2line.keyPressEvent(self.find_text, event)
+
+    def perform_find_next(self):
+        self.q2code.findFirst(self.find_text.get_text(), False, False, False, False, True)
+        self.last_find_direction = "down"
+
+    def perform_find_prev(self):
+        line1, index1, line2, index2 = self.q2code.getSelection()
+        self.q2code.setCursorPosition(line1, index1)
+        self.q2code.findFirst(self.find_text.get_text(), False, False, False, False, False)
+        self.last_find_direction = "up"
+
+    def create_replace(self):
+        self.replace_frame = QWidget()
+        self.replace_frame.setLayout(QHBoxLayout())
+        self.replace_frame.layout().setContentsMargins(0, 0, 0, 0)
+        self.replace_text = q2line({})
+        self.replace_text.returnPressed.connect(self.perform_replace)
+
+        self.replace_frame.layout().addWidget(q2label({"label": "replace:"}))
+        self.replace_frame.layout().addWidget(self.replace_text)
+
+        self.replace_button = q2button({"label": "Ok"})
+        self.replace_button.pressed.connect(self.perform_replace)
+        self.replace_button.set_fixed_width(3, "w")
+        self.replace_frame.layout().addWidget(self.replace_button)
+
+    def perform_replace(self):
+        self.q2code.replace(self.replace_text.get_text())
+        if self.last_find_direction == "down":
+            self.perform_find_next()
         else:
-            self.statusBar().hide()
+            self.perform_find_prev()
 
-    def is_statusbar_visible(self):
-        return self.statusBar().isVisible()
+    def create_go(self):
+        self.go_frame = QWidget()
+        self.go_frame.setLayout(QHBoxLayout())
+        self.go_frame.layout().setContentsMargins(0, 0, 0, 0)
+        self.go_text = q2line({"datatype": "int", "datalen": 5, "num": 1})
+        self.go_frame.layout().addWidget(q2label({"label": "go to line:"}))
+        self.go_frame.layout().addWidget(self.go_text)
+        self.go_button = q2button({"label": ">"})
+        self.go_button.set_fixed_width(3, "w")
+        self.go_frame.layout().addWidget(self.go_button)
+        self.go_frame.layout().addStretch()
+        self.go_text.editingFinished.connect(self.perform_go)
+        self.go_button.pressed.connect(self.perform_go)
+
+    def perform_go(self):
+        self.q2code.goto_line(self.go_text.get_text())
+
+    def show_find(self):
+        st = self.q2code.selectedText()
+        if st:
+            self.find_text.set_text(st)
+        self.find_frame.show()
+        self.replace_frame.hide()
+        self.go_frame.hide()
+        self.find_text.set_focus()
+        self.show()
 
-    def get_char_width(self, char="w"):
-        return QFontMetrics(self.font()).horizontalAdvance(char)
+    def show_replace(self):
+        self.find_frame.show()
+        self.replace_frame.show()
+        self.go_frame.hide()
+        self.show()
 
-    def get_char_height(self):
-        return QFontMetrics(self.font()).height()
-
-    @staticmethod
-    def get_open_file_dialoq(header=q2app.DIALOG_OPEN_FILE_TITLE, path="", filter=""):
-        if path == "":
-            path = os.path.expanduser("~/Desktop")
-        rez = QFileDialog.getOpenFileName(None, header, path, filter)
-        return rez
-
-    def _get_open_file_dialoq(self, header=q2app.DIALOG_OPEN_FILE_TITLE, path="", filter=""):
-        if self._last_get_file_path and not path:
-            path = self._last_get_file_path
-        rez = Q2App.get_open_file_dialoq(header, path, filter)
-        if rez:
-            self._last_get_file_path = os.path.dirname(rez[0])
-        QApplication.setActiveWindow(self)
-        return rez
-
-    @staticmethod
-    def get_save_file_dialoq(header=q2app.DIALOG_SAVE_FILE_TITLE, path="", filter="", confirm_overwrite=True):
-        if path == "":
-            path = os.path.expanduser("~/Desktop")
-        if confirm_overwrite:
-            rez = QFileDialog.getSaveFileName(None, header, path, filter)
-        else:
-            rez = QFileDialog.getSaveFileName(
-                None, header, path, filter, options=QFileDialog.Option.DontConfirmOverwrite
-            )
-        return rez
-
-    def _get_save_file_dialoq(
-        self, header=q2app.DIALOG_SAVE_FILE_TITLE, path="", filter="", confirm_overwrite=True
-    ):
-        if self._last_get_file_path and not path:
-            path = self._last_get_file_path
-        rez = Q2App.get_save_file_dialoq(header, path, filter, confirm_overwrite)
-        if rez:
-            self._last_get_file_path = os.path.dirname(rez[0])
-        QApplication.setActiveWindow(self)
-        return rez
-
-    def _wait_for_show(self):
-        while QApplication.activeWindow() is None:
-            QTimer.singleShot(100, self._wait_for_show)
-            return
-        self.process_events()
-        self.add_new_tab()
-        self.process_events()
-        self.on_start()
-
-    def keyboard_modifiers(self):
-        modifiers = QApplication.keyboardModifiers()
-        rez = []
-        if modifiers == Qt.KeyboardModifier.ShiftModifier:
-            rez.append("shift")
-        elif modifiers == Qt.KeyboardModifier.ControlModifier:
-            rez.append("control")
-        elif modifiers == (Qt.KeyboardModifier.AltModifier):
-            rez.append("alt")
-        return "+".join(rez)
-
-    def save_geometry(self, settings):
-        Q2QtWindow.save_geometry(self, settings)
-
-    def run(self):
-        # self.restore_geometry(self.settings)
-        Q2QtWindow.restore_geometry(self, self.settings)
+    def show_go(self):
+        self.find_frame.hide()
+        self.replace_frame.hide()
+        self.go_frame.show()
+        self.go_text.set_alignment(9)
+        self.go_text.set_text("")
+        self.go_text.set_focus()
         self.show()
-        super().run()
-        self._wait_for_show()
-        if len(QApplication.allWindows()) == 1:
-            QApplication.instance().exec()
-
-    def add_new_tab(self):
-        self.q2_tabwidget.addTab()
-
-    def show(self):
-        QMainWindow.show(self)
-
-    def on_new_tab(self):
-        return super().on_new_tab()
-
-    def showEvent(self, event):
-        event.accept()
-        super().showEvent(event)
-
-    def closeEvent(self, event: QEvent):
-        if not self.closing:
-            self.close()
-        event.accept()
-
-    def close(self):
-        self.closing = True
-        super().close()
-        QApplication._mw_count -= 1
-        QMainWindow.close(self)
-        if QApplication._mw_count <= 0:
-            os._exit(0)
+
+    def set_find_text(self, text=""):
+        self.find_text.set_text(text)
+        self.find_text.set_focus()
+
+    def show(self) -> None:
+        self.set_geometry()
+        return super().show()
+
+    def set_geometry(self):
+        parent = self.q2code
+        rect = parent.rect()
+        self.setFixedWidth(400 if rect.width() > 400 else int(rect.width() / 2))
+        pos = rect.topLeft()
+        pos.setX(rect.width() - self.width())
+        pos = parent.mapToGlobal(pos)
+        self.move(pos)
```

### Comparing `q2gui-0.1.96/q2gui/pyqt6/q2form.py` & `q2gui-0.1.97/q2gui/pyqt6/q2form.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/q2model.py` & `q2gui-0.1.97/q2gui/pyqt6/q2model.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/q2style.py` & `q2gui-0.1.97/q2gui/pyqt6/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/q2widget.py` & `q2gui-0.1.97/q2gui/pyqt6/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/q2window.py` & `q2gui-0.1.97/q2gui/pyqt6/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/__init__.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2button.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2button.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2check.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2check.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2code.py` & `q2gui-0.1.97/q2gui/q2model.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,425 +8,456 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-import sys
-
 if __name__ == "__main__":
+    import sys
 
     sys.path.insert(0, ".")
 
     from demo.demo import demo
 
     demo()
 
-# from PyQt6.QtWidgets import QTextEdit, QSizePolicy
-from PyQt6.QtWidgets import (
-    QVBoxLayout,
-    QHBoxLayout,
-    QWidget,
-)
-
-from PyQt6.Qsci import QsciScintilla, QsciLexerPython, QsciLexerSQL, QsciLexerJSON, QsciAPIs, QsciLexer
-from PyQt6.QtGui import QColor
-
-# from PyQt6.QtWidgets import QMenu
-from PyQt6.QtCore import Qt, QTimer, QSize
-
-from q2gui.pyqt6.q2widget import Q2Widget
-from q2gui.pyqt6.widgets.q2line import q2line
-from q2gui.pyqt6.widgets.q2label import q2label
-from q2gui.pyqt6.widgets.q2button import q2button
-from q2gui.q2utils import int_
-
-
-class q2code(QsciScintilla, Q2Widget):
-    def __init__(self, meta):
-        super().__init__(meta)
-        self.setUtf8(True)
-        self.setFolding(QsciScintilla.FoldStyle.BoxedTreeFoldStyle)
-
-        self.lexer: QsciLexer = None
-        self.set_lexer()
-        self.set_background_color()
-
-        self.setAutoIndent(True)
-        self.setIndentationGuides(True)
-        self.setIndentationsUseTabs(False)
-        self.setBraceMatching(QsciScintilla.BraceMatch.StrictBraceMatch)
-        self.setMarginLineNumbers(1, True)
-        self.setMarginWidth(1, "9999")
-        self.setTabWidth(4)
-
-        self.setAutoCompletionSource(QsciScintilla.AutoCompletionSource.AcsAll)
-        self.setAutoCompletionCaseSensitivity(True)
-        self.setAutoCompletionReplaceWord(True)
-        self.setAutoCompletionThreshold(1)
-
-        self.SCN_DOUBLECLICK
-
-        self.setCaretLineVisible(True)
-
-        self.searchIndicator = QsciScintilla.INDIC_CONTAINER
-        self.SendScintilla(QsciScintilla.SCI_INDICSETSTYLE, self.searchIndicator, QsciScintilla.INDIC_BOX)
-        self.SendScintilla(QsciScintilla.SCI_INDICSETFORE, self.searchIndicator, QColor("red"))
-
-        self.cursorPositionChanged.connect(self.__cursorPositionChanged)
-        self.__markOccurrencesTimer = QTimer(self)
-        self.__markOccurrencesTimer.setSingleShot(True)
-        self.__markOccurrencesTimer.setInterval(500)
-        self.__markOccurrencesTimer.timeout.connect(self.__markOccurrences)
-        self.textChanged.connect(self.valid)
-        # self.setContextMenuPolicy(Qt.ContextMenuPolicy.ActionsContextMenu)
-        self.editor_panel = q2editor_panel(self)
-        self.create_context_menu()
-        self.set_custom_autocompletition_list()
-
-    def set_lexer(self, lexer=""):
-        if lexer == "":
-            lexer = self.meta["control"]
-        if "python" in lexer:
-            self.lexer = QsciLexerPython()
-        elif "sql" in lexer:
-            self.lexer = QsciLexerSQL()
-        elif "json" in lexer:
-            self.lexer = QsciLexerJSON()
-        else:
-            self.lexer = QsciLexerPython()
-        if self.lexer:
-            self.setLexer(self.lexer)
-
-    def set_custom_autocompletition_list(self, custom_autocompletions_list=[]):
-        custom_autocompletions_list = self.meta["form"].q2_app.get_autocompletition_list()
-        self.__api = QsciAPIs(self.lexer)
-        for ac in custom_autocompletions_list:
-            self.__api.add(ac)
-        self.__api.prepare()
-
-    def set_background_color(self, red=150, green=200, blue=230):
-        # color_mode = self.meta.get("q2_app").q2style.get_system_color_mode()
-        # print(color_mode, self.meta.get("q2_app").q2style.color_mode)
-        # b_color = QColor(self.meta.get("q2_app").q2style.styles.get(color_mode).get("background"))
-        # f_color = QColor(self.meta.get("q2_app").q2style.styles.get(color_mode).get("color"))
-
-        # self.setMatchedBraceForegroundColor(QColor("lightgreen"))
-        self.lexer.setDefaultPaper(QColor(red, green, blue))
-        self.lexer.setPaper(QColor(red, green, blue))
-        # self.lexer.setDefaultPaper(b_color)
-        # self.lexer.setPaper(b_color)
-        # self.lexer.setColor(f_color, 5)
-        self.setMarginsForegroundColor(QColor("black"))
-        self.setMarginsBackgroundColor(QColor("gray"))
-
-    def __cursorPositionChanged(self, line, index):
-        self.__markOccurrencesTimer.stop()
-        self.clearIndicatorRange(
-            0, 0, self.lines() - 1, len(self.text(self.lines() - 1)), self.searchIndicator
-        )
-        self.__markOccurrencesTimer.start()
+import csv
+import datetime
+import re
+
+import q2gui.q2app as q2app
+from q2gui.q2utils import num
+
+try:
+    from q2db.cursor import Q2Cursor
+    from q2db.db import Q2Db
+except Exception:
+    pass
+
+
+class Q2Model:
+    def __init__(self):
+        self.q2_form = None
+        self.columns = []
+        self.headers = []
+        self.alignments = []
+
+        self.records = []
+        self.proxy_records = []
+        self.use_proxy = False
+        self.relation_cache = {}
+        self.lastdata_error_text = ""
+
+        self.meta = []
+        self.cursor = None
+
+        # CRUD flags
+        self.readonly = True
+        self.delete_enabled = False
+        self.insert_enabled = False
+        self.update_enabled = False
+
+        self.filterable = False
+
+        self.data_changed = False
+
+        self.order_text = ""
+        self.where_text = ""
+
+    def get_row(self, row_number):
+        if row_number < len(self.records):
+            return self.records[row_number]
+        else:
+            return None
 
-    def __findFirstTarget(self, text):
-        if text == "":
-            return False
-        self.__targetSearchExpr = text.encode("utf-8")
-        self.__targetSearchFlags = QsciScintilla.SCFIND_MATCHCASE | QsciScintilla.SCFIND_WHOLEWORD
-        self.__targetSearchStart = 0
-        self.__targetSearchEnd = self.SendScintilla(QsciScintilla.SCI_GETTEXTLENGTH)
-        self.__targetSearchActive = True
-        return self.__doSearchTarget()
+    def get_table_name(self):
+        return ""
 
-    def __findNextTarget(self):
-        if not self.__targetSearchActive:
-            return False
-        return self.__doSearchTarget()
+    def get_data_error(self):
+        return self.lastdata_error_text
 
-    def __doSearchTarget(self):
-        if self.__targetSearchStart == self.__targetSearchEnd:
-            self.__targetSearchActive = False
-            return False
-        self.SendScintilla(QsciScintilla.SCI_SETTARGETSTART, self.__targetSearchStart)
-        self.SendScintilla(QsciScintilla.SCI_SETTARGETEND, self.__targetSearchEnd)
-        self.SendScintilla(QsciScintilla.SCI_SETSEARCHFLAGS, self.__targetSearchFlags)
-        pos = self.SendScintilla(
-            QsciScintilla.SCI_SEARCHINTARGET, len(self.__targetSearchExpr), self.__targetSearchExpr
-        )
-        if pos == -1:
-            self.__targetSearchActive = False
-            return False
-        self.SendScintilla(QsciScintilla.SCI_INDICATORFILLRANGE, pos, len(self.__targetSearchExpr))
-        targend = self.SendScintilla(QsciScintilla.SCI_GETTARGETEND)
-        self.__targetSearchStart = targend
+    def set_data_error(self, text=""):
+        self.lastdata_error_text = text
+
+    def update(self, record: dict, current_row, refresh=True):
+        if self.proxy_records:
+            current_row = self.proxy_records[current_row]
+        if self.records:
+            self.records[current_row].update(record)
+        self.data_changed = True
+        if refresh:
+            self.refresh()
         return True
 
-    def __markOccurrences(self):
-        if self.hasFocus():
-            line, index = self.getCursorPosition()
-            ok = self.__findFirstTarget(self.__getWord(self.text(line), index - 1))
-            while ok:
-                ok = self.__findNextTarget()
-
-    def __getWord(self, text, index):
-        word = ""
-        for x in range(index, -1, -1):
-            if text[x].isalpha() or text[x].isdigit():
-                word = text[x] + word
-            else:
-                break
-        for x in range(index + 1, len(text)):
-            if text[x].isalpha() or text[x].isdigit():
-                word += text[x]
-            else:
-                break
-        return word
+    def insert(self, record: dict, current_row=0, refresh=True):
+        self.records.append(record)
+        self.data_changed = True
+        if refresh:
+            self.refresh()
+        return True
 
-    def mouseDoubleClickEvent(self, event):
-        return super().mouseDoubleClickEvent(event)
+    def delete(self, row_number, refresh=True):
+        if self.proxy_records:
+            row_number = self.proxy_records[row_number]
+        self.records.pop(row_number)
+        self.data_changed = True
+        if refresh:
+            self.refresh()
+        return True
 
-    def create_context_menu(self):
-        self.context_menu = self.createStandardContextMenu()
-        self.context_menu.addSeparator()
-
-        find_action = self.context_menu.addAction("Find")
-        find_action.triggered.connect(self.editor_panel.show_find)
-        find_action.setShortcuts(["Ctrl+F", "F3"])
-
-        replace_action = self.context_menu.addAction("Replace")
-        replace_action.triggered.connect(self.editor_panel.show_replace)
-        replace_action.setShortcut("Ctrl+H")
-
-        gotoline_action = self.context_menu.addAction("Go to line")
-        gotoline_action.triggered.connect(self.editor_panel.show_go)
-        gotoline_action.setShortcut("Ctrl+G")
-
-        self.context_menu.addSeparator()
-
-        fold_action = self.context_menu.addAction("Fold/Unfold")
-        fold_action.triggered.connect(self.perform_folding)
-        fold_action.setShortcuts(["Alt+Up", "Alt+Down"])
-
-        foldall_action = self.context_menu.addAction("Fold/Unfold All")
-        foldall_action.triggered.connect(self.foldAll)
-        foldall_action.setShortcuts(["Alt+Left", "Alt+Right"])
-
-        self.context_menu.addSeparator()
-        comment_action = self.context_menu.addAction("Comment/uncomment line(s)")
-        comment_action.setShortcut("Ctrl+3")
-        comment_action.triggered.connect(self.perform_comment)
-
-        complete_action = self.context_menu.addAction("Autocomplete")
-        complete_action.triggered.connect(self.autoCompleteFromAll)
-        complete_action.setShortcuts(["Ctrl+Space"])
-
-        self.addActions(self.context_menu.actions())
-        for x in self.context_menu.actions():
-            if x.isEnabled():
-                x.setVisible(True)
+    def set_where(self, where_text=""):
+        self.where_text = where_text
+        if self.where_text:
+            self.use_proxy = True
+            self.proxy_records = []
+            for row, rec in enumerate(self.records):
+                rc = dict(rec)
+                if eval(self.where_text, rc):
+                    self.proxy_records.append(row)
+        else:
+            self.use_proxy = False
+        self.refresh()
+        return self
+
+    def get_where(self):
+        return self.where_text
+
+    def set_order(self, order_data=""):
+        if isinstance(order_data, int):
+            self.order_text = self.columns[order_data]
+        elif isinstance(order_data, list):
+            self.order_text = ",".join(order_data)
+        else:
+            self.order_text = order_data
+        if self.records:
+            colname = self.order_text
+
+            if self.proxy_records:
+                sort_records = {}
+                for x in range(len(self.proxy_records)):
+                    value = self.records[self.proxy_records[x]][colname]
+                    if value not in sort_records:
+                        sort_records[value] = [self.proxy_records[x]]
+                    else:
+                        sort_records[value].append(self.proxy_records[x])
             else:
-                x.setVisible(False)
+                sort_records = {}
+                for x in range(len(self.records)):
+                    if self.records[x][colname] not in sort_records:
+                        sort_records[self.records[x][colname]] = [x]
+                    else:
+                        sort_records[self.records[x][colname]].append(x)
+
+            sorted_keys = sorted([x for x in sort_records.keys()])
+            # sorted_keys.sort()
+            tmp_proxy_records = []
+            for x in sorted_keys:
+                for y in sort_records[x]:
+                    tmp_proxy_records.append(y)
+
+            self.proxy_records = tmp_proxy_records
+            self.use_proxy = True
+
+    def get_order(self):
+        return self.order_text
+
+    def refresh(self):
+        self.relation_cache = {}
+
+    def reset(self):
+        self.records = []
+        self.proxy_records = []
+        self.use_proxy = False
+        self.relation_cache = {}
+        self.lastdata_error_text = ""
+
+    def set_records(self, records):
+        self.records = records
+
+    def build(self):
+        self.columns = []
+        self.headers = []
+        self.alignments = []
+        self.meta = []
+        for meta in self.q2_form.controls:
+            if meta.get("column", "").startswith("/") or meta.get("nogrid"):
+                # if meta.get("column", "").startswith("/"):
+                continue
+            if meta.get("control", "") in ["button", "widget", "form"]:
+                continue
+            self.q2_form.model.add_column(meta)
+
+    def add_column(self, meta):
+        if not meta.get("control"):
+            meta["control"] = "line"
+
+        meta = q2app.Q2Controls.validate(meta)
+        self.columns.append(meta["column"])
+        self.headers.append(meta["gridlabel" if meta.get("gridlabel") else "label"])
+        self.alignments.append(meta.get("alignment", "7"))
+        self.meta.append(meta)
+
+    def get_record(self, row):
+        if row < 0 or row > len(self.records) - 1:
+            return {}
+        if self.use_proxy:
+            return self.records[self.proxy_records[row]]
+        else:
+            return self.records[row]
 
-    def perform_comment(self):
-        selected_lines = []
-        current_line, current_pos = self.getCursorPosition()
-        if self.hasSelectedText():
-            line1, pos1, line2, pos2 = self.getSelection()
-            for x in range(line1, line2 + 1):
-                selected_lines.append(x)
-        else:
-            selected_lines.append(current_line)
-
-        for line in selected_lines:
-            new_pos = self.comment_line(line, current_pos)
-            if line == current_line:
-                self.setCursorPosition(current_line, new_pos)
-
-        if len(selected_lines) > 1:
-            self.setSelection(line1, pos1, line2, pos2)
-
-    def comment_line(self, line, pos):
-        current_line = self.text(line)
-        if len(current_line.strip()):
-            if current_line.lstrip()[0:2] == "# ":
-                comment_pos = current_line.index("# ")
-                if comment_pos < pos:
-                    pos -= 2
-                self.setSelection(line, comment_pos, line, comment_pos + 2)
-                self.removeSelectedText()
-            else:
-                spaces_count = len(current_line) - len(current_line.lstrip())
-                if pos > spaces_count:
-                    pos += 2
-                self.insertAt("# ", line, spaces_count)
-        return pos
-
-    def perform_folding(self):
-        self.foldLine(self.getCursorPosition()[0])
-
-    def current_line(self):
-        return self.getCursorPosition()[0]
-
-    def goto_line(self, line=0):
-        self.setCursorPosition(int_(line) - 1, 0)
-        self.set_focus()
-        self.ensureLineVisible(self.getCursorPosition()[0])
-        self.editor_panel.close()
-
-    def contextMenuEvent(self, event):
-        self.create_context_menu()
-        self.context_menu.exec(event.globalPos())
-
-    def showEvent(self, ev):
-        self.updateGeometry()
-        return super().showEvent(ev)
-
-    def sizeHint(self):
-        if self.isVisible():
-            return QSize(99999, 99999)
-        else:
-            return super().sizeHint()
-
-
-class q2editor_panel(QWidget):
-    def __init__(self, parent, text=""):
-        super().__init__(parent, Qt.WindowType.Popup)
-        # super().__init__(parent)
-        self.setLayout(QVBoxLayout())
-
-        self.layout().setContentsMargins(0, 0, 0, 0)
-        # self.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
-        self.create_find()
-        self.create_replace()
-        self.create_go()
-
-        self.layout().addWidget(self.find_frame)
-        self.layout().addWidget(self.replace_frame)
-        self.layout().addWidget(self.go_frame)
-
-        self.set_find_text(text)
-        self.q2code: q2code = parent
-        self.last_find_direction = "down"
-
-    def create_find(self):
-        self.find_frame = QWidget()
-
-        self.find_frame.setLayout(QHBoxLayout())
-        self.find_frame.layout().setContentsMargins(0, 0, 0, 0)
-
-        self.find_next_button = q2button({"label": ">"})
-        self.find_next_button.set_fixed_width(3, "w")
-
-        self.find_prev_button = q2button({"label": "<"})
-        self.find_prev_button.set_fixed_width(3, "w")
-
-        self.find_text = q2line({})
-        self.find_frame.layout().addWidget(q2label({"label": "find:"}))
-        self.find_frame.layout().addWidget(self.find_text)
-        self.find_frame.layout().addWidget(self.find_prev_button)
-        self.find_frame.layout().addWidget(self.find_next_button)
-        self.find_next_button.pressed.connect(self.perform_find_next)
-        self.find_prev_button.pressed.connect(self.perform_find_prev)
-        self.find_text.keyPressEvent = self.find_keyPressEvent
-
-    def find_keyPressEvent(self, event):
-        if event.key() in [Qt.Key.Key_Up] or (
-            event.key() in [Qt.Key.Key_Enter, Qt.Key.Key_Return, Qt.Key.Key_F3]
-            and event.modifiers() == Qt.KeyboardModifier.ShiftModifier
-        ):
-            self.perform_find_prev()
-        elif event.key() in [Qt.Key.Key_Enter, Qt.Key.Key_Return, Qt.Key.Key_Down, Qt.Key.Key_F3]:
-            self.perform_find_next()
-        elif event.key() == Qt.Key.Key_H:
-            self.show_replace()
-        q2line.keyPressEvent(self.find_text, event)
-
-    def perform_find_next(self):
-        self.q2code.findFirst(self.find_text.get_text(), False, False, False, False, True)
-        self.last_find_direction = "down"
-
-    def perform_find_prev(self):
-        line1, index1, line2, index2 = self.q2code.getSelection()
-        self.q2code.setCursorPosition(line1, index1)
-        self.q2code.findFirst(self.find_text.get_text(), False, False, False, False, False)
-        self.last_find_direction = "up"
-
-    def create_replace(self):
-        self.replace_frame = QWidget()
-        self.replace_frame.setLayout(QHBoxLayout())
-        self.replace_frame.layout().setContentsMargins(0, 0, 0, 0)
-        self.replace_text = q2line({})
-        self.replace_text.returnPressed.connect(self.perform_replace)
-
-        self.replace_frame.layout().addWidget(q2label({"label": "replace:"}))
-        self.replace_frame.layout().addWidget(self.replace_text)
-
-        self.replace_button = q2button({"label": "Ok"})
-        self.replace_button.pressed.connect(self.perform_replace)
-        self.replace_button.set_fixed_width(3, "w")
-        self.replace_frame.layout().addWidget(self.replace_button)
-
-    def perform_replace(self):
-        self.q2code.replace(self.replace_text.get_text())
-        if self.last_find_direction == "down":
-            self.perform_find_next()
-        else:
-            self.perform_find_prev()
-
-    def create_go(self):
-        self.go_frame = QWidget()
-        self.go_frame.setLayout(QHBoxLayout())
-        self.go_frame.layout().setContentsMargins(0, 0, 0, 0)
-        self.go_text = q2line({"datatype": "int", "datalen": 5, "num": 1})
-        self.go_frame.layout().addWidget(q2label({"label": "go to line:"}))
-        self.go_frame.layout().addWidget(self.go_text)
-        self.go_button = q2button({"label": ">"})
-        self.go_button.set_fixed_width(3, "w")
-        self.go_frame.layout().addWidget(self.go_button)
-        self.go_frame.layout().addStretch()
-        self.go_text.editingFinished.connect(self.perform_go)
-        self.go_button.pressed.connect(self.perform_go)
-
-    def perform_go(self):
-        self.q2code.goto_line(self.go_text.get_text())
-
-    def show_find(self):
-        st = self.q2code.selectedText()
-        if st:
-            self.find_text.set_text(st)
-        self.find_frame.show()
-        self.replace_frame.hide()
-        self.go_frame.hide()
-        self.find_text.set_focus()
-        self.show()
-
-    def show_replace(self):
-        self.find_frame.show()
-        self.replace_frame.show()
-        self.go_frame.hide()
-        self.show()
-
-    def show_go(self):
-        self.find_frame.hide()
-        self.replace_frame.hide()
-        self.go_frame.show()
-        self.go_text.set_alignment(9)
-        self.go_text.set_text("")
-        self.go_text.set_focus()
-        self.show()
-
-    def set_find_text(self, text=""):
-        self.find_text.set_text(text)
-        self.find_text.set_focus()
-
-    def show(self) -> None:
-        self.set_geometry()
-        return super().show()
-
-    def set_geometry(self):
-        parent = self.q2code
-        rect = parent.rect()
-        self.setFixedWidth(400 if rect.width() > 400 else int(rect.width() / 2))
-        pos = rect.topLeft()
-        pos.setX(rect.width() - self.width())
-        pos = parent.mapToGlobal(pos)
-        self.move(pos)
+    def _get_related(self, value, meta, do_not_show_value=False, reset_cache=False):
+        if meta.get("num") and num(value) == 0:
+            return ""
+        elif value == "":
+            return ""
+        key = (meta["to_table"], f"{meta['to_column']}='{value}'", meta["related"])
+        if not reset_cache and key in self.relation_cache:
+            related = self.relation_cache[key]
+        else:
+            related = self.get_related(meta["to_table"], f"{meta['to_column']}='{value}'", meta["related"])
+            self.relation_cache[key] = related
+        if related is None or related == {}:
+            related = ""
+        if do_not_show_value:
+            return f"{related}"
+        else:
+            return f"{value},{related}"
+
+    def get_related(self, to_table, filter, related):
+        return "get_related"
+
+    def data(self, row, col, role="display"):
+        if role == "display":
+            colName = self.columns[col]
+            value = self.get_record(row).get(colName, "")
+            meta = self.meta[col]
+            if meta.get("relation"):
+                value = self._get_related(value, meta)
+            elif meta.get("show"):
+                value = meta.get("show")(mode="grid", row=row)
+            elif self.is_strign_for_num(meta):
+                if num(value) == 0:
+                    value = 1
+                value = meta.get("pic").split(";")[int(num(value)) - 1]
+            elif meta.get("num"):  # Numeric value
+                if num(value) == 0:  # do not show zero
+                    value = ""
+                elif meta.get("pic") == "F":  # financial format
+                    format_string = q2app.FINANCIAL_FORMAT % meta.get("datadec", 0)
+                    value = format_string.format(num(value))
+            elif meta["datatype"] == "date":
+                try:
+                    value = datetime.datetime.strptime(value, "%Y-%m-%d").strftime(q2app.DATE_FORMAT_STRING)
+                except Exception:
+                    value = ""
+            return value
+
+    def is_strign_for_num(self, meta):
+        """return str data from numeric controls - radio, list, combo"""
+        return meta.get("num") and ("radio" in meta["control"] or meta["control"] in ("list", "combo"))
+
+    def alignment(self, col):
+        if self.meta[col].get("relation"):
+            return 7
+        elif self.is_strign_for_num(self.meta[col]):
+            return 7
+        return self.alignments[col]
+
+    def column_header_data(self, col):
+        return self.headers[col]
+
+    def row_header_data(self, row):
+        return f"{row}"
+
+    def row_count(self):
+        if self.use_proxy:
+            return len(self.proxy_records)
+        else:
+            return len(self.records)
+
+    def column_count(self):
+        return len(self.columns)
+
+    def parse_lookup_text(self, text):
+        text = text.upper()
+        raw_cond_list = ["+"] + re.split("([+-])", text)
+        cond_list = []
+        for cond in range(int(len(raw_cond_list) / 2)):
+            operator = raw_cond_list[cond * 2]
+            value = raw_cond_list[cond * 2 + 1]
+            if operator and value:
+                cond_list.append([operator, value])
+        return cond_list
+
+    def lookup(self, column, text):
+        """search for text in column, return list of [row, value]"""
+        cond_list = self.parse_lookup_text(text)
+        rez = []
+        for x in range(self.row_count()):
+            cond_result = True
+            for cond in cond_list:
+                operator = cond[0]
+                value = cond[1]
+                model_value = self.get_record(x)[self.columns[column]]
+                if self.meta[column].get("relation"):
+                    model_value = self._get_related(model_value, self.meta[column])
+
+                if operator == "+" and value not in model_value.upper():
+                    cond_result = False
+                elif operator == "-" and value in model_value.upper():
+                    cond_result = False
+            if cond_result:
+                rez.append([x, model_value])
+        return rez
+
+    def data_export(self, file):
+        pass
+
+    def data_import(self, file):
+        pass
+
+    def seek_row(self, row_dict):
+        pk = self.get_meta_primary_key()
+        if pk and pk in row_dict:
+            for row_number in range(self.row_count()):
+                rec_dic = self.get_record(row_number)
+                if str(row_dict[pk]) == rec_dic[pk]:
+                    return row_number
+        else:
+            for row_number in range(self.row_count()):
+                rec_dic = self.get_record(row_number)
+                found = 1
+                for colname in row_dict:
+                    if row_dict[colname] != rec_dic[colname]:
+                        found = 0
+                        break
+                if found:
+                    return row_number
+        return 0
+
+    def get_meta_primary_key(self):
+        for x in self.q2_form.controls:
+            if x["pk"]:
+                return x["column"]
+
+    def get_uniq_value(self, column, value):
+        pass
+
+    def get_next_sequence(self, column, start_value=0):
+        pass
+
+
+class Q2CsvModel(Q2Model):
+    def __init__(self, csv_file_object=None):
+        super().__init__()
+        csv_dict = csv.DictReader(csv_file_object)
+        # If there are names with space -  replace spaces in columns names
+        if [filename for filename in csv_dict.fieldnames if " " in filename]:
+            fieldnames = [x.replace(" ", "_") for x in csv_dict.fieldnames]
+            csv_dict = csv.DictReader(csv_file_object, fieldnames)
+        self.set_records([x for x in csv_dict])
+        self.filterable = True
+
+
+class Q2CursorModel(Q2Model):
+    def __init__(self, cursor: Q2Cursor = None):
+        super().__init__()
+        self.cursor = cursor
+
+        self.readonly = False
+        self.delete_enabled = False
+        self.insert_enabled = False
+        self.update_enabled = False
+        self.set_where(self.cursor.where)
+        self.set_order(self.cursor.order)
+
+    def get_table_name(self):
+        return self.cursor.table_name
+
+    def row_count(self):
+        return self.cursor.row_count()
+
+    def get_record(self, row):
+        return self.cursor.record(row)
+
+    def refresh(self):
+        super().refresh()
+        self.cursor.refresh()
+
+    def get_uniq_value(self, column, value):
+        return self.cursor.get_uniq_value(column, value)
+
+    def get_next_sequence(self, column, start_value=0):
+        return self.cursor.get_next_sequence(column, start_value)
+
+    def delete(self, current_row=0, refresh=True):
+        self.set_data_error()
+        record = self.get_record(current_row)
+        if self.cursor.delete(record, refresh=False):
+            if refresh:
+                self.refresh()
+            return True
+        else:
+            self.set_data_error(self.cursor.last_sql_error())
+            return False
+
+    def update(self, record: dict, current_row=0, refresh=True):
+        self.set_data_error()
+        if self.cursor.update(record, refresh=False):
+            if refresh:
+                self.refresh()
+            return True
+        else:
+            self.set_data_error(f"{self.cursor.last_sql_error()}<br>{self.cursor.last_sql()}")
+            return False
+
+    def insert(self, record: dict, current_row=0, refresh=True):
+        self.set_data_error()
+        if self.cursor.insert(record, refresh=False):
+            if refresh:
+                self.refresh()
+            return True
+        else:
+            self.set_data_error(self.cursor.last_sql_error())
+            return False
+
+    def get_related(self, to_table, filter, related):
+        db: Q2Db = self.cursor.q2_db
+        return db.get(to_table, filter, related)
+
+    def set_order(self, order_data):
+        if self.cursor.table_name:
+            super().set_order(order_data=order_data)
+            self.cursor.set_order(self.order_text)
+        return self
+
+    def set_where(self, where_text=""):
+        self.cursor.set_where(where_text)
+        self.refresh()
+        return super().set_where(where_text)
+
+    def add_column(self, meta):
+        """update metadata from db"""
+        db: Q2Db = self.cursor.q2_db
+        db_meta = db.db_schema.get_schema_table_attr(self.cursor.table_name, meta["column"])
+        meta["pk"] = db_meta.get("pk", "")
+        meta["datatype"] = db_meta.get("datatype", meta["datatype"])
+        if num(meta["datalen"]) < num(db_meta.get("datalen", 10)):
+            meta["datalen"] = int(num(db_meta.get("datalen", 10)))
+        if "datadec" not in meta:
+            meta["datadec"] = int(num(db_meta.get("datadec", 2)))
+        return super().add_column(meta)
+
+    def data_export(self, file: str, tick_callback=None):
+        if file.lower().endswith(".csv"):
+            self.cursor.export_csv(file, tick_callback=tick_callback)
+        else:
+            self.cursor.export_json(file, tick_callback=tick_callback)
+
+    def data_import(self, file: str, tick_callback=None):
+        if file.lower().endswith(".csv"):
+            rez = self.cursor.import_csv(file, tick_callback=tick_callback)
+        else:
+            rez = self.cursor.import_json(file, tick_callback=tick_callback)
+        self.refresh()
+        return rez
```

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2combo.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2combo.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2date.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2date.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2doublespin.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2doublespin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2frame.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2frame.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2grid.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2grid.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2image.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2image.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2label.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2label.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2line.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2line.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2list.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2list.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2lookup.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2lookup.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2progressbar.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2progressbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2radio.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2radio.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2relation.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2relation.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2scroller.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2scroller.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2sheet.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2sheet.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2space.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2space.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2spin.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2spin.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2tab.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2tab.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2text.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2text.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2toolbar.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2toolbar.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/pyqt6/widgets/q2toolbutton.py` & `q2gui-0.1.97/q2gui/pyqt6/widgets/q2toolbutton.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/q2app.py` & `q2gui-0.1.97/q2gui/q2app.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/q2dialogs.py` & `q2gui-0.1.97/q2gui/q2dialogs.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/q2form.py` & `q2gui-0.1.97/q2gui/q2form.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     demo()
 
 import q2gui.q2app as q2app
 from q2gui.q2model import Q2Model
 from q2gui.q2utils import int_, num
 import re
+import html
 import json
 import gettext
 
 _ = gettext.gettext
 
 
 VIEW = "VIEW"
@@ -495,15 +496,15 @@
         buttons.add_control("/")
 
         self.system_controls = buttons
 
     def add_crud_buttons(self, mode):
         buttons = q2app.Q2Controls()
         buttons.add_control("/")
-        buttons.add_control("/h", "-")
+        buttons.add_control("/h", "-", tag="crud_buttons")
         if not self.no_view_action:
             buttons.add_control(
                 column="_prev_button",
                 label="<",
                 control="button",
                 mess="prev record",
                 valid=lambda: self.move_crud_view(8),
@@ -984,16 +985,16 @@
         Q2BulkUpdate(self)
 
     def grid_data_info(self):
         columns = self.model.columns
         self._q2dialogs.q2Mess(
             f"{q2app.GRID_DATA_INFO_TABLE}: {self.model.get_table_name()}"
             f"<br>{q2app.GRID_DATA_INFO_ROWS}: {self.model.row_count()}"
-            f"<br>{q2app.GRID_DATA_INFO_ORDER}: {self.model.order_text}"
-            f"<br>{q2app.GRID_DATA_INFO_FILTER}: {self.model.where_text}"
+            f"<br>{q2app.GRID_DATA_INFO_ORDER}: {self.model.get_order()}"
+            f"<br>{q2app.GRID_DATA_INFO_FILTER}: {html.escape(self.model.get_where())}"
             f"<br>{q2app.GRID_DATA_INFO_COLUMNS}: {columns}"
         )
 
     def set_style_sheet(self, css: str):
         self.style_sheet = css
         for x in self.form_stack:
             x.set_style_sheet(self.style_sheet)
```

### Comparing `q2gui-0.1.96/q2gui/q2style.py` & `q2gui-0.1.97/q2gui/q2style.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/q2utils.py` & `q2gui-0.1.97/q2gui/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/q2widget.py` & `q2gui-0.1.97/q2gui/q2widget.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/q2gui/q2window.py` & `q2gui-0.1.97/q2gui/q2window.py`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/README.md` & `q2gui-0.1.97/README.md`

 * *Files identical despite different names*

### Comparing `q2gui-0.1.96/PKG-INFO` & `q2gui-0.1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2gui
-Version: 0.1.96
+Version: 0.1.97
 Summary: Python GUI toolkit
 License: Apache 2.0
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

