# Comparing `tmp/medit-0.0.4.tar.gz` & `tmp/medit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medit-0.0.4.tar", max compression
+gzip compressed data, was "medit-0.0.5.tar", max compression
```

## Comparing `medit-0.0.4.tar` & `medit-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     2188 2023-07-02 16:12:39.541375 medit-0.0.4/Readme.md
--rw-r--r--   0        0        0        0 2023-06-18 13:03:52.329049 medit-0.0.4/medit/__init__.py
--rwxr-xr-x   0        0        0     2392 2023-07-02 11:33:38.540816 medit-0.0.4/medit/cli.py
--rw-r--r--   0        0        0     2101 2023-07-02 15:49:58.797871 medit-0.0.4/medit/medit.ui
--rw-r--r--   0        0        0     4732 2023-07-02 15:46:12.488227 medit-0.0.4/medit/meditor.py
--rw-r--r--   0        0        0     7340 2023-07-02 16:11:41.761127 medit-0.0.4/medit/mview.py
--rw-r--r--   0        0        0        0 2023-07-02 15:40:29.959990 medit-0.0.4/medit/styles/__init__.py
--rw-r--r--   0        0        0    18966 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/github-markdown-dark.css
--rw-r--r--   0        0        0    18979 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/github-markdown-light.css
--rw-r--r--   0        0        0     5061 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/pygments-solarized-style/solarized-dark.css
--rw-r--r--   0        0        0     5061 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/pygments-solarized-style/solarized-light.css
--rw-r--r--   0        0        0    36899 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/solarized-dark-all-sites.css
--rw-r--r--   0        0        0    36890 2023-07-02 11:33:38.542816 medit-0.0.4/medit/styles/external/solarized-light-all-sites.css
--rw-r--r--   0        0        0     4282 2023-07-02 11:33:38.542816 medit-0.0.4/medit/styles/external/thomasf-solarized-css/solarized-dark.css
--rw-r--r--   0        0        0     4282 2023-07-02 11:33:38.542816 medit-0.0.4/medit/styles/external/thomasf-solarized-css/solarized-light.css
--rwxr-xr-x   0        0        0     6985 2023-07-02 15:43:07.140557 medit-0.0.4/medit/ui.py
--rw-r--r--   0        0        0     2389 2023-07-02 11:32:00.577590 medit-0.0.4/medit/utils.py
--rw-r--r--   0        0        0     2315 2023-07-02 16:11:41.762127 medit-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3129 1970-01-01 00:00:00.000000 medit-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2328 2023-07-03 06:21:56.302488 medit-0.0.5/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-16 07:35:55.912297 medit-0.0.5/medit/__init__.py
+-rwxr-xr-x   0        0        0     2192 2023-07-03 06:21:56.302488 medit-0.0.5/medit/cli.py
+-rw-r--r--   0        0        0     2362 2023-07-03 06:51:24.784057 medit-0.0.5/medit/medit.ui
+-rw-r--r--   0        0        0     5064 2023-07-03 07:10:06.510948 medit-0.0.5/medit/meditor.py
+-rw-r--r--   0        0        0     7517 2023-07-03 06:21:56.302488 medit-0.0.5/medit/mview.py
+-rw-r--r--   0        0        0        0 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/__init__.py
+-rw-r--r--   0        0        0    18966 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/github-markdown-dark.css
+-rw-r--r--   0        0        0    18979 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/github-markdown-light.css
+-rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/pygments-solarized-style/solarized-dark.css
+-rw-r--r--   0        0        0     5061 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/pygments-solarized-style/solarized-light.css
+-rw-r--r--   0        0        0    36899 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/solarized-dark-all-sites.css
+-rw-r--r--   0        0        0    36890 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/solarized-light-all-sites.css
+-rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/thomasf-solarized-css/solarized-dark.css
+-rw-r--r--   0        0        0     4282 2023-07-03 06:21:56.302488 medit-0.0.5/medit/styles/external/thomasf-solarized-css/solarized-light.css
+-rwxr-xr-x   0        0        0     8338 2023-07-03 06:21:56.302488 medit-0.0.5/medit/ui.py
+-rw-r--r--   0        0        0     5023 2023-07-03 06:21:56.302488 medit-0.0.5/medit/utils.py
+-rwxr-xr-x   0        0        0     6266 2023-06-29 19:10:09.897127 medit-0.0.5/medit/yatl.py
+-rw-r--r--   0        0        0     2315 2023-07-03 07:18:17.940235 medit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3269 1970-01-01 00:00:00.000000 medit-0.0.5/PKG-INFO
```

### Comparing `medit-0.0.4/Readme.md` & `medit-0.0.5/Readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,23 +31,28 @@
 python3 -m pip install --user --upgrade dist/pocketrockit-0.0.25-py3-none-any.whl
 ```
 
 ## 1.0 TODO
 
 * [x] File to title
 * [x] File viewer for Plain, Python, YAML, JSON, ..
-* [x] Save
+* [x] Autosave
+* [ ] Autoload
+* [ ] Change into / step up current directory
+* [ ] Zen mode
+* [ ] Recent files
+* [ ] Search/open files
+* [ ] Search in files
 * [ ] Preview for Markdown/.. only
-* [ ] Manage word wrap
+* [ ] Manage word wrap in editor
 * [ ] Hightlight todo.txt
 * [ ] Notify external file changes
 * [ ] (Re-)store zoom and fullscreen
 * [ ] File ignore filter
 * [ ] Icon
-* [ ] Autoload
 * [ ] Proper Qt style
 * [ ] Show local images
 * [ ] Show remote images
 * [ ] Slim file / folder create / rename
 * [ ] Proper View CSS selector
 * [ ] View follows editor
 * [ ] Links clickable
```

### Comparing `medit-0.0.4/medit/cli.py` & `medit-0.0.5/medit/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,24 +17,18 @@
 from medit.utils import setup_logging
 
 
 def parse_args(argv: Sequence[str] | None = None) -> Args:
     """Cool git like multi command argument parser"""
     parser = ArgumentParser(__doc__)
     parser.add_argument("--verbose", "-v", action="store_true")
+    parser.add_argument("--info", action="store_true")
 
     parser.set_defaults(func=fn_ui)
-    subparsers = parser.add_subparsers(help="available commands", metavar="CMD")
-
-    parser_help = subparsers.add_parser("help")
-    parser_help.set_defaults(func=lambda *_: parser.print_help())
-
-    parser_ui = subparsers.add_parser("ui")
-    parser_ui.set_defaults(func=fn_ui)
-    parser_ui.add_argument("path", type=Path, nargs="?")
+    parser.add_argument("path", type=Path, nargs="?")
 
     return parser.parse_args(argv)
 
 
 def logger() -> logging.Logger:
     """Named logger"""
     return logging.getLogger("medit.cli")
@@ -75,13 +69,13 @@
 
 def fn_ui(args: Args) -> None:
     ui_main(args.path if hasattr(args, "path") else None)
 
 
 def main() -> int:
     """Entry point for everything else"""
-    (args := parse_args()).func(args)
-    return 0
+    args = parse_args()
+    return fn_info(args) if args.info else fn_ui(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `medit-0.0.4/medit/medit.ui` & `medit-0.0.5/medit/medit.ui`

 * *Files 12% similar despite different names*

#### Comparing `medit-0.0.4/medit/medit.ui` & `medit-0.0.5/medit/medit.ui`

```diff
@@ -16,52 +16,63 @@
         <verstretch>0</verstretch>
       </sizepolicy>
     </property>
     <property name="windowTitle">
       <string>medit</string>
     </property>
     <widget class="QWidget" name="centralwidget">
-      <layout class="QGridLayout" name="gridLayout">
-        <item row="0" column="0" colspan="2">
-          <layout class="QHBoxLayout" name="horizontalLayout">
-            <property name="leftMargin">
-              <number>0</number>
+      <layout class="QHBoxLayout" name="horizontalLayout_2">
+        <property name="leftMargin">
+          <number>0</number>
+        </property>
+        <property name="topMargin">
+          <number>0</number>
+        </property>
+        <property name="rightMargin">
+          <number>0</number>
+        </property>
+        <property name="bottomMargin">
+          <number>0</number>
+        </property>
+        <item>
+          <widget class="QSplitter" name="gb_splitter">
+            <property name="orientation">
+              <enum>Qt::Horizontal</enum>
             </property>
-            <property name="topMargin">
-              <number>0</number>
-            </property>
-            <property name="rightMargin">
-              <number>0</number>
-            </property>
-            <property name="bottomMargin">
-              <number>0</number>
-            </property>
-            <item>
-              <widget class="QSplitter" name="gb_splitter">
-                <property name="orientation">
-                  <enum>Qt::Horizontal</enum>
-                </property>
-                <widget class="QTreeView" name="tv_files"/>
-                <widget class="MEditor" name="txt_editor"/>
-                <widget class="MView" name="wv_rendered" native="true">
-                  <property name="minimumSize">
-                    <size>
-                      <width>100</width>
-                      <height>0</height>
-                    </size>
-                  </property>
-                  <property name="url" stdset="0">
-                    <url>
-                      <string>about:blank</string>
-                    </url>
-                  </property>
-                </widget>
-              </widget>
-            </item>
-          </layout>
+            <widget class="QSplitter" name="gb_left_splitter">
+              <property name="orientation">
+                <enum>Qt::Vertical</enum>
+              </property>
+              <layout class="QVBoxLayout" name="verticalLayout">
+                <item>
+                  <widget class="QTreeView" name="tv_files"/>
+                </item>
+                <item>
+                  <widget class="QListWidget" name="lst_recent"/>
+                </item>
+                <item>
+                  <widget class="QPlainTextEdit" name="txt_log"/>
+                </item>
+              </layout>
+            </widget>
+            <widget class="MEditor" name="txt_editor"/>
+            <widget class="MView" name="wv_rendered" native="true">
+              <property name="minimumSize">
+                <size>
+                  <width>100</width>
+                  <height>0</height>
+                </size>
+              </property>
+              <property name="url" stdset="0">
+                <url>
+                  <string>about:blank</string>
+                </url>
+              </property>
+            </widget>
+          </widget>
         </item>
       </layout>
     </widget>
   </widget>
   <customwidgets>
     <customwidget>
       <class>MView</class>
```

### Comparing `medit-0.0.4/medit/meditor.py` & `medit-0.0.5/medit/meditor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 #!/usr/bin/env python3
 # https://stackoverflow.com/questions/40002373/qscintilla-based-text-editor-in-pyqt5-with-clickable-functions-and-variables
 
-from PyQt6 import Qsci, QtGui, QtCore
-from PyQt6.QtGui import QImage, QPainter
 from pathlib import Path
 
+from PyQt6 import Qsci, QtCore, QtGui
+from PyQt6.QtGui import QImage, QPainter
+
+
 class MEditor(Qsci.QsciScintilla):
     def __init__(self, parent=None):
         super().__init__(parent)
         self.setIndentationsUseTabs(False)
         self.setIndentationWidth(4)
 
         font = QtGui.QFont()
-        font.setFamily("DejaVu Sans Mono")
+        font.setFamily("Source Code Pro Semibold")
+        if font.exactMatch():
+            print("Font set successfully")
+        else:
+            print("Font not found, using closest match", font.family())
         font.setFixedPitch(True)
-        font.setPointSize(14)
+        font.setPointSize(20)
         self.setFont(font)
         self.setMarginsFont(font)
         # self.zoomIn()
         # self.zoomOut()
 
         # Margin 0 is used for line numbers
         fontmetrics = QtGui.QFontMetrics(font)
         self.setMarginsFont(font)
-        self.setMarginWidth(0, fontmetrics.maxWidth() + 6)#.width("000") + 6)
-        self.setMarginLineNumbers(0, True)
-        #self.setMarginsBackgroundColor(QtGui.QColor("#cccccc"))
-        #self.setMarginBackgroundColor(1, QtGui.QColor("lightgray"))
-
+        self.setMarginWidth(0, fontmetrics.boundingRect("000").width()+ 6)
+        #self.setMarginLineNumbers(0, True)
+        self.setMarginsBackgroundColor(QtGui.QColor("#eee8d5"))
+        self.setMarginsForegroundColor(QtGui.QColor("#93a1a1"))
+        # self.setMarginBackgroundColor(1, QtGui.QColor("lightgray"))
 
         # self._marker = None
         # Clickable margin 1 for showing markers
         # self.setMarginSensitivity(1, True)
         # self.connect(self,
         #    SIGNAL('marginClicked(int, int, Qt::KeyboardModifiers)'),
         #    self.on_margin_clicked)
@@ -47,57 +53,61 @@
         self.SendScintilla(Qsci.QsciScintilla.SCI_STYLESETFONT, 1, "Courier".encode())
 
         # Don't want to see the horizontal scrollbar at all
         # Use raw message to Scintilla here (all messages are documented
         # here: http://www.scintilla.org/ScintillaDoc.html)
         self.SendScintilla(Qsci.QsciScintilla.SCI_SETHSCROLLBAR, 0)
 
-        self.setWrapMode(self.WrapMode.WrapWord)
+        #self.setWrapMode(self.WrapMode.WrapWord)
+        self.setWrapMode(self.WrapMode.WrapNone)
         self.setEolMode(self.EolMode.EolUnix)
         self.setEolVisibility(False)
         self.setWhitespaceVisibility(self.WhitespaceVisibility.WsVisible)
 
-
-        #self.image = QImage("logo_mk.png")
-        #painter = QPainter()
-        #painter.begin(self.image)
-        #painter.setCompositionMode(QPainter.CompositionMode.CompositionMode_DestinationIn)
-        #painter.fillRect(self.image.rect(), QtGui.QColor(0, 0, 0, 100))
-        #painter.end()
-
-    #def paintEvent(self, e):
-        #painter = QPainter()
-        #painter.begin(self.viewport())
-        #painter.drawImage(QtCore.QPoint(0, 0), self.image)
-        #painter.end()
-        #super().paintEvent(e)
+        # self.image = QImage("logo_mk.png")
+        # painter = QPainter()
+        # painter.begin(self.image)
+        # painter.setCompositionMode(QPainter.CompositionMode.CompositionMode_DestinationIn)
+        # painter.fillRect(self.image.rect(), QtGui.QColor(0, 0, 0, 100))
+        # painter.end()
+
+    # def paintEvent(self, e):
+    # painter = QPainter()
+    # painter.begin(self.viewport())
+    # painter.drawImage(QtCore.QPoint(0, 0), self.image)
+    # painter.end()
+    # super().paintEvent(e)
 
     def openFile(self, path):
         suffix = path.suffix.lower().strip("~")
         lexer = (
-            Qsci.QsciLexerMarkdown() if suffix in {".md", ".markdown"} else
-            Qsci.QsciLexerYAML() if suffix in {".yaml", ".yml"} else
-            Qsci.QsciLexerBash() if suffix in {".sh"} else
-            Qsci.QsciLexerPython() if suffix in {".py"} else
-            Qsci.QsciLexerXML() if suffix in {".xml", ".svg"} else
-            None
+            Qsci.QsciLexerMarkdown()
+            if suffix in {".md", ".markdown"}
+            else Qsci.QsciLexerYAML()
+            if suffix in {".yaml", ".yml"}
+            else Qsci.QsciLexerBash()
+            if suffix in {".sh"}
+            else Qsci.QsciLexerPython()
+            if suffix in {".py"}
+            else Qsci.QsciLexerXML()
+            if suffix in {".xml", ".svg"}
+            else None
         )
         if lexer:
             lexer.setFont(self.font())
-            #lexer.setPaper(QtGui.QColor("#073642"))
-            #lexer.setDefaultPaper(QtGui.QColor("#073642"))
+            # lexer.setPaper(QtGui.QColor("#073642"))
+            # lexer.setDefaultPaper(QtGui.QColor("#073642"))
             lexer.setPaper(QtGui.QColor("#fdf6e3"))
             lexer.setDefaultPaper(QtGui.QColor("#fdf6e3"))
 
         self.setLexer(lexer)
 
         with open(path) as textFile:
             self.setText(textFile.read())
 
-
     def view_state(self):
         # In Qt5/PyQt5 how do I restore exact visible area and cursor
         #  position of QTextEdit?:
         # https://stackoverflow.com/questions/67751888
 
         # relative approach
         # try:
```

### Comparing `medit-0.0.4/medit/mview.py` & `medit-0.0.5/medit/mview.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,140 +1,138 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 
+import pygments.lexers
 from markdown import markdown
-from PyQt6.QtWebEngineWidgets import QWebEngineView
 from pygments import highlight
-import pygments.lexers
 from pygments.formatters import HtmlFormatter
+from PyQt6.QtWebEngineWidgets import QWebEngineView
 
 
 class MView(QWebEngineView):
     def __init__(self, parent):
         super().__init__(parent)
         self.css_content_markdown = "".join(
             f"<style>{open(Path(__file__).parent / path).read()}</style>"
             for path in (
                 "styles/external/github-markdown-light.css",
                 "styles/external/thomasf-solarized-css/solarized-light.css",
                 "styles/external/solarized-light-all-sites.css",
                 "styles/external/pygments-solarized-style/solarized-light.css",
-
-                #"styles/external/github-markdown-dark.css",
-                #"styles/external/thomasf-solarized-css/solarized-dark.css",
-                #"styles/external/solarized-dark-all-sites.css",
-                #"styles/external/pygments-solarized-style/solarized-dark.css",
-            ))
+                # "styles/external/github-markdown-dark.css",
+                # "styles/external/thomasf-solarized-css/solarized-dark.css",
+                # "styles/external/solarized-dark-all-sites.css",
+                # "styles/external/pygments-solarized-style/solarized-dark.css",
+            )
+        )
 
         self.css_content = "".join(
             f"<style>{open(Path(__file__).parent / path).read()}</style>"
-            for path in (
-                "styles/external/pygments-solarized-style/solarized-light.css",
-            ))
+            for path in ("styles/external/pygments-solarized-style/solarized-light.css",)
+        )
 
         self.css_content_unused = "".join(
             f"<style>{open(Path(__file__).parent / path).read()}</style>"
             for path in (
                 #
                 # Basic markdown stuff
                 #
-
                 # GitHub - html only
-                #"styles/external/github-markdown-light.css",
-                #"styles/external/github-markdown-dark.css",
-
+                # "styles/external/github-markdown-light.css",
+                # "styles/external/github-markdown-dark.css",
                 # dark - https://nihaojob.github.io/markdown-css-smartisan/
-                #"styles/external/github-markdown.css",
-
+                # "styles/external/github-markdown.css",
                 # html only, fonts not affected `.markdown` class
                 # https://cdn.jsdelivr.net/npm/@naokim03/markdown-theme-solarized@1.0.2/
-                #"styles/markdown.min.css",
-
+                # "styles/markdown.min.css",
                 # https://github.com/alphapapa/solarized-everything-css
-                #"styles/external/solarized-light-all-sites.css",
-                #"styles/external/solarized-dark-all-sites.css",
-
+                # "styles/external/solarized-light-all-sites.css",
+                # "styles/external/solarized-dark-all-sites.css",
                 # html only
-                #https://github.com/thomasf/solarized-css
+                # https://github.com/thomasf/solarized-css
                 # "styles/solarized-light.css",
-                #"styles/solarized-dark.css",  #               | light, transparent, decent
-
+                # "styles/solarized-dark.css",  #               | light, transparent, decent
                 #
                 # Pygments
                 #
-
                 # pygments via `pygments-solarized-style`
-                #"styles/external/solarized-light.css",  #               | light, transparent, decent
-                #"styles/external/solarized-dark.css",  #               | light, transparent, decent
-
+                # "styles/external/solarized-light.css",  #               | light, transparent, decent
+                # "styles/external/solarized-dark.css",  #               | light, transparent, decent
                 # pygments defaults
-                #"styles/pygments/abap.css",  #               | light, transparent, decent
-                #"styles/pygments/algol.css",  #              | light/dark, transparent, bw
-                #"styles/pygments/algol_nu.css",  #           | light/dark, transparent, bw
-                #"styles/pygments/arduino.css",  #            | light/dark, decent
-                #"styles/pygments/autumn.css",  #             | light (dark)
-                #"styles/pygments/borland.css",  #            | light
-                #"styles/pygments/bw.css",  #                 |
-                #"styles/pygments/colorful.css",  #           | light +string
-                #"styles/pygments/default.css",  #            |
-                #"styles/pygments/dracula.css",  #            | dark
-                #"styles/pygments/emacs.css",  #              |
-                #"styles/pygments/friendly.css",  #           |
-                #"styles/pygments/friendly_grayscale.css",  # |
-                #"styles/pygments/fruity.css",  #             | dark
-                #"styles/pygments/igor.css",  #               | light (dark)
-                #"styles/pygments/inkpot.css",  #             | dark (light) +strings
-                #"styles/pygments/lilypond.css",  #           | light dark
-                #"styles/pygments/lovelace.css",  #           | light dark
-                #"styles/pygments/manni.css",  #              | dark light +nice
-                #"styles/pygments/material.css",  #           | dark
-                #"styles/pygments/monokai.css",  #            | dark
-                #"styles/pygments/murphy.css",  #             |
-                #"styles/pygments/native.css",  #             |
-                #"styles/pygments/nord.css",  #               |
-                #"styles/pygments/pastie.css",  #             |
-                #"styles/pygments/perldoc.css",  #            |
-                #"styles/pygments/rainbow_dash.css",  #       |
-                #"styles/pygments/rrt.css",  #                |
-                #"styles/pygments/sas.css",  #                |
-                #"styles/pygments/staroffice.css",  #         |
-                #"styles/pygments/tango.css",  #              |
-                #"styles/pygments/trac.css",  #               | light dark
-                #"styles/pygments/vim.css",  #                |
-                #"styles/pygments/vs.css",  #                 | light, transparent, decent
-                #"styles/pygments/xcode.css",  #              | light, transparent, decent
-                #"styles/pygments/zenburn.css",  #            | dark
+                # "styles/pygments/abap.css",  #               | light, transparent, decent
+                # "styles/pygments/algol.css",  #              | light/dark, transparent, bw
+                # "styles/pygments/algol_nu.css",  #           | light/dark, transparent, bw
+                # "styles/pygments/arduino.css",  #            | light/dark, decent
+                # "styles/pygments/autumn.css",  #             | light (dark)
+                # "styles/pygments/borland.css",  #            | light
+                # "styles/pygments/bw.css",  #                 |
+                # "styles/pygments/colorful.css",  #           | light +string
+                # "styles/pygments/default.css",  #            |
+                # "styles/pygments/dracula.css",  #            | dark
+                # "styles/pygments/emacs.css",  #              |
+                # "styles/pygments/friendly.css",  #           |
+                # "styles/pygments/friendly_grayscale.css",  # |
+                # "styles/pygments/fruity.css",  #             | dark
+                # "styles/pygments/igor.css",  #               | light (dark)
+                # "styles/pygments/inkpot.css",  #             | dark (light) +strings
+                # "styles/pygments/lilypond.css",  #           | light dark
+                # "styles/pygments/lovelace.css",  #           | light dark
+                # "styles/pygments/manni.css",  #              | dark light +nice
+                # "styles/pygments/material.css",  #           | dark
+                # "styles/pygments/monokai.css",  #            | dark
+                # "styles/pygments/murphy.css",  #             |
+                # "styles/pygments/native.css",  #             |
+                # "styles/pygments/nord.css",  #               |
+                # "styles/pygments/pastie.css",  #             |
+                # "styles/pygments/perldoc.css",  #            |
+                # "styles/pygments/rainbow_dash.css",  #       |
+                # "styles/pygments/rrt.css",  #                |
+                # "styles/pygments/sas.css",  #                |
+                # "styles/pygments/staroffice.css",  #         |
+                # "styles/pygments/tango.css",  #              |
+                # "styles/pygments/trac.css",  #               | light dark
+                # "styles/pygments/vim.css",  #                |
+                # "styles/pygments/vs.css",  #                 | light, transparent, decent
+                # "styles/pygments/xcode.css",  #              | light, transparent, decent
+                # "styles/pygments/zenburn.css",  #            | dark
             )
         )
 
     def show(self, content, highlight_mode):
 
         if highlight_mode == ".md":
-            html, style = markdown(
-                content,
-                extensions=[
-                    "extra",
-                    "codehilite",
-                    "markdown_checklist.extension",
-                ],
-            ), self.css_content_markdown
+            html, style = (
+                markdown(
+                    content,
+                    extensions=[
+                        "extra",
+                        "codehilite",
+                        "markdown_checklist.extension",
+                    ],
+                ),
+                self.css_content_markdown,
+            )
         else:
-            formatter =  HtmlFormatter(linenos="table", cssclass="codehilite")
+            formatter = HtmlFormatter(linenos="table", cssclass="codehilite")
             lexer = (
-                pygments.lexers.YamlLexer() if highlight_mode in {".yaml", ".yml"} else
-                pygments.lexers.BashLexer() if highlight_mode in {".sh"} else
-                pygments.lexers.PythonLexer() if highlight_mode in {".py"} else
-                pygments.lexers.XmlLexer() if highlight_mode in {".xml", ".svg", ".lbrn2"} else
-                pygments.lexers.TexLexer()
+                pygments.lexers.YamlLexer()
+                if highlight_mode in {".yaml", ".yml"}
+                else pygments.lexers.BashLexer()
+                if highlight_mode in {".sh"}
+                else pygments.lexers.PythonLexer()
+                if highlight_mode in {".py"}
+                else pygments.lexers.XmlLexer()
+                if highlight_mode in {".xml", ".svg", ".lbrn2"}
+                else pygments.lexers.TexLexer()
             )
 
             html, style = highlight(content, lexer, formatter), self.css_content
 
-#        print(html)
+        #        print(html)
         self.setHtml(
             f"""
 <!doctype html>
 <html lang="en">
   <meta charset="utf-8"><head>{style}</head></meta>
   <body class="markdown-body markdown">{html}</body>
 </html>
```

### Comparing `medit-0.0.4/medit/styles/external/github-markdown-dark.css` & `medit-0.0.5/medit/styles/external/github-markdown-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.4/medit/styles/external/github-markdown-light.css` & `medit-0.0.5/medit/styles/external/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.4/medit/styles/external/pygments-solarized-style/solarized-dark.css` & `medit-0.0.5/medit/styles/external/pygments-solarized-style/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.4/medit/styles/external/pygments-solarized-style/solarized-light.css` & `medit-0.0.5/medit/styles/external/pygments-solarized-style/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.4/medit/styles/external/solarized-dark-all-sites.css` & `medit-0.0.5/medit/styles/external/solarized-dark-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.4/medit/styles/external/solarized-light-all-sites.css` & `medit-0.0.5/medit/styles/external/solarized-light-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.4/medit/styles/external/thomasf-solarized-css/solarized-dark.css` & `medit-0.0.5/medit/styles/external/thomasf-solarized-css/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.4/medit/styles/external/thomasf-solarized-css/solarized-light.css` & `medit-0.0.5/medit/styles/external/thomasf-solarized-css/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.4/medit/ui.py` & `medit-0.0.5/medit/ui.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 import json
 import logging
 import os
 import signal
 import sys
 from contextlib import suppress
 from pathlib import Path
-
+import asyncio
 from PyQt6 import QtCore, QtGui, QtWidgets, uic
 from PyQt6.QtWebEngineWidgets import QWebEngineView
+from medit.utils import fs_changes, watchdog, setup_logging
+import qdarktheme
 
 CFG_FILE = "~/.medit.cfg"
 
 
 def log() -> logging.Logger:
     """Returns the local logger"""
     return logging.getLogger("medit.ui")
@@ -32,16 +34,16 @@
 
 class MEditWindow(QtWidgets.QMainWindow):
     """The one and only application window"""
 
     def __init__(self, path: Path | None) -> None:
         super().__init__()
         uic.loadUi(Path(__file__).parent / "medit.ui", self)
-        #self.setStyleSheet(styleSheet)
-        #self.setStyleSheet("background-color: yellow;")
+        # self.setStyleSheet(styleSheet)
+        # self.setStyleSheet("background-color: yellow;")
 
         # css =  open(Path(__file__).parent / "github-markdown-light.css").read()
         # print(css)
         # self.wv_rendered.setStyleSheet(css)
         # self.setAcceptDrops(True)
         # self.config = qrm_common.load_json(qrm_common.CFG_FILE)
 
@@ -50,16 +52,28 @@
         config = load_default(CFG_FILE, {})
 
         self.autosave_timer = QtCore.QTimer(self)
         self.autosave_timer.timeout.connect(self.on_autosave_timer_timeout)
 
         self.setGeometry(*config.get("window_geometry", (50, 50, 1000, 500)))
         self.base_dir = (
-            path and (path if path.is_dir else path.parent) or Path(config.get("base_dir") or ".")
+            path
+            and (path if path.is_dir else path.parent)
+            or Path(config.get("base_dir") or ".").absolute()
         )
+        self.autoload_thread = QtCore.QThread(self)
+        self.autoload_thread.run = lambda: self.async_stuff()
+        self.autoload_thread.start()
+
+        #self.fs_watcher = QtCore.QFileSystemWatcher([self.base_dir.as_posix()])
+        #self.fs_watcher.fileChanged.connect(self.on_file_changed_externally)
+        #self.fs_watcher.directoryChanged.connect(self.on_file_changed_externally)
+        #self.fs_watcher.addPaths([self.base_dir.as_posix()])
+        #print(self.fs_watcher.files())
+
         self.fs_model = QtGui.QFileSystemModel()
         self.fs_model.setRootPath(Path.home().as_posix())
 
         self.open_file = None
 
         self.set_open_file(path if path and path.is_file() else config.get("open_file"))
 
@@ -68,48 +82,71 @@
         self.tv_files.setModel(self.fs_model)
 
         self.tv_files.selectionModel().selectionChanged.connect(self.on_tv_files_selectionChanged)
 
         self.tv_files.hideColumn(1)
         self.tv_files.hideColumn(2)
         self.tv_files.hideColumn(3)
-        self.tv_files.setRootIndex(self.fs_model.index(Path.home().as_posix()))
-        self.tv_files.expand(self.fs_model.index(self.base_dir.absolute().as_posix()))
+        self.tv_files.setRootIndex(self.fs_model.index(self.base_dir.as_posix()))
+        self.tv_files.expand(self.fs_model.index(self.base_dir.as_posix()))
         if self.open_file:
             self.tv_files.setCurrentIndex(self.fs_model.index(self.open_file.absolute().as_posix()))
         else:
             self.tv_files.setCurrentIndex(self.fs_model.index(self.base_dir.absolute().as_posix()))
 
         self.show()
 
+    def async_stuff(self):
+        print("Async")
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+        #terminator = threading.Event()
+
+        # https://stackoverflow.com/a/71956673
+        _tasks = {
+            asyncio.ensure_future(self.watch_fs_changes())
+        }
+        loop.run_forever()
+
+    @watchdog
+    async def watch_fs_changes(self) -> None:
+        """Observe changes to filesystem and mark walls dirty"""
+        async for changed_path in fs_changes(self.base_dir, timeout=1, postpone=True):
+            log().info("file %s changed", changed_path)
+            QtCore.QMetaObject.invokeMethod(
+                self, "on_file_changed_externally", QtCore.Qt.QueuedConnection,
+                #QtCore.Q_ARG(list, [])
+            )
+
 
     def reset_timer(self):
         logging.debug("reset modification timer")
         self.autosave_timer.start(300)
 
     def render_content(self):
-        self.wv_rendered.show(self.txt_editor.text(), self.open_file and self.open_file.suffix.strip("~"))
-
+        self.wv_rendered.show(
+            self.txt_editor.text(), self.open_file and self.open_file.suffix.strip("~")
+        )
 
     def on_autosave_timer_timeout(self):
         """"""
         self.autosave_timer.stop()
         self.render_content()
         self.save()
 
     def save(self):
-        #if not self.dirty:
-            #return
+        # if not self.dirty:
+        # return
         log().info("save to %s", self.open_file)
-        #self.dirty = True
+        # self.dirty = True
         text_to_save = self.txt_editor.text()
         if not text_to_save:
             log().warning("I don't dare to overwrite with empty content..")
             return
-        open(self.open_file, 'w').write(text_to_save)
+        open(self.open_file, "w").write(text_to_save)
 
     def set_open_file(self, path):
         self.open_file = None
         block_state = self.txt_editor.blockSignals(True)
         selected_file = Path(path) if path else None
         if not path:
             return
@@ -119,29 +156,31 @@
         except UnicodeDecodeError:
             self.txt_editor.setText("")
         finally:
             self.txt_editor.blockSignals(block_state)
             self.setWindowTitle(str(self.open_file))
         self.render_content()
 
-    #def on_tv_files_clicked(self, index) -> None:
-        #selected_path = Path(self.fs_model.filePath(index))
-        #if selected_path.is_file():
-            #self.set_open_file(selected_path)
-
     def on_tv_files_selectionChanged(self, selection) -> None:
-        #print(Path(self.fs_model.filePath(selection.indexes()[0])))
-        selected_path = Path(self.fs_model.filePath(selection.indexes()[0]))
-        if selected_path.is_file():
-            self.set_open_file(selected_path)
+        # print(Path(self.fs_model.filePath(selection.indexes()[0])))
+        try:
 
+            selected_path = Path(self.fs_model.filePath(selection.indexes()[0]))
+            if selected_path.is_file():
+                self.set_open_file(selected_path)
+        except IndexError:
+            print("FILE REMOVED?")
 
     def on_txt_editor_textChanged(self) -> None:
         self.reset_timer()
 
+    @QtCore.pyqtSlot(str)
+    def on_file_changed_externally(file) -> None:
+        print(file)
+
     def event(self, event: QtCore.QEvent) -> bool:
         # if event.type() == QtCore.QEvent.DragEnter:
         # if any(
         # Path(u.url()).suffix.lower() in {".pdf", ".epub"} for u in event.mimeData().urls()
         # ):
         # event.accept()
         # elif event.type() == QtCore.QEvent.Drop:
@@ -187,18 +226,15 @@
             open(os.path.expanduser(CFG_FILE), "w"),
         )
 
 
 def main(path: Path) -> None:
     """Typical PyQt5 boilerplate main entry point"""
 
-    import qdarktheme
-
-
-    logging.getLogger().setLevel(logging.INFO)
+    setup_logging()
     app = QtWidgets.QApplication(sys.argv)
 
     qdarktheme.setup_theme("light")
 
     window = MEditWindow(path)
 
     for s in (signal.SIGABRT, signal.SIGINT, signal.SIGSEGV, signal.SIGTERM):
```

### Comparing `medit-0.0.4/pyproject.toml` & `medit-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medit"
-version = "0.0.4"
+version = "0.0.5"
 description = "Markup Editor"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/medit.git"
 readme = "Readme.md"
 packages = [
   {include = "medit/**/*.py"},
   {include = "medit/**/*.ui"},
```

### Comparing `medit-0.0.4/PKG-INFO` & `medit-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Markup Editor
 Home-page: https://projects.om-office.de/frans/medit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -55,23 +55,28 @@
 python3 -m pip install --user --upgrade dist/pocketrockit-0.0.25-py3-none-any.whl
 ```
 
 ## 1.0 TODO
 
 * [x] File to title
 * [x] File viewer for Plain, Python, YAML, JSON, ..
-* [x] Save
+* [x] Autosave
+* [ ] Autoload
+* [ ] Change into / step up current directory
+* [ ] Zen mode
+* [ ] Recent files
+* [ ] Search/open files
+* [ ] Search in files
 * [ ] Preview for Markdown/.. only
-* [ ] Manage word wrap
+* [ ] Manage word wrap in editor
 * [ ] Hightlight todo.txt
 * [ ] Notify external file changes
 * [ ] (Re-)store zoom and fullscreen
 * [ ] File ignore filter
 * [ ] Icon
-* [ ] Autoload
 * [ ] Proper Qt style
 * [ ] Show local images
 * [ ] Show remote images
 * [ ] Slim file / folder create / rename
 * [ ] Proper View CSS selector
 * [ ] View follows editor
 * [ ] Links clickable
```

