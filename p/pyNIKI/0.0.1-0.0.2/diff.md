# Comparing `tmp/pyniki-0.0.1.tar.gz` & `tmp/pyniki-0.0.2.tar.gz`

## Comparing `pyniki-0.0.1.tar` & `pyniki-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyniki-0.0.1/src/pyniki/__init__.py
--rw-r--r--   0        0        0    24381 2020-02-02 00:00:00.000000 pyniki-0.0.1/src/pyniki/main.py
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyniki-0.0.1/LICENSE
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyniki-0.0.1/README.md
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pyniki-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 pyniki-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyniki-0.0.2/src/pyniki/__init__.py
+-rw-r--r--   0        0        0    25319 2020-02-02 00:00:00.000000 pyniki-0.0.2/src/pyniki/main.py
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 pyniki-0.0.2/LICENSE
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyniki-0.0.2/README.md
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 pyniki-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 pyniki-0.0.2/PKG-INFO
```

### Comparing `pyniki-0.0.1/src/pyniki/main.py` & `pyniki-0.0.2/src/pyniki/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import atexit
 import copy
 import curses
 import glob
 import os
+import pathlib
 import pickle
 import subprocess
 import sys
 import time
 import traceback
 
 scr = None
@@ -29,15 +30,15 @@
     scr.clear()
 
 def _teardown():
     curses.nocbreak()
     scr.keypad(False)
     curses.echo()
     curses.curs_set(curs_state)
-    # curses.endwin()
+    curses.endwin()
 
 def draw_frame(height, width, offset_y=0, offset_x=0, active=False):
     attr = curses.A_BOLD if active else curses.A_NORMAL
     scr.addstr(offset_y, offset_x,
                '╒' + '═' * (width-2) + '╕', attr)
     for i in range(height-2):
         scr.addstr(offset_y+i+1, offset_x,
@@ -242,29 +243,39 @@
             key = scr.getch()
             if key in range(ord('a'), ord('z')+1) or key in range(ord('0'), ord('9')+1):
                 key = chr(key).upper()
                 txt = txt[:pos] + key + txt[pos+1:]
                 if pos+1 < 12:
                     pos += 1
             elif key == curses.KEY_RIGHT:
-                if pos+1 < 12:
+                if pos+1 < 12 and txt[pos] != '_':
                     pos += 1
             elif key == curses.KEY_LEFT:
                 if pos > 0:
                     pos -= 1
+            elif key == curses.KEY_BACKSPACE:
+                if pos > 0:
+                    pos -= 1
+                    txt = txt[:pos] + txt[pos+1:] + '_'
+            elif key == curses.KEY_DC:
+                if txt[pos] != '_':
+                    txt = txt[:pos] + txt[pos+1:] + '_'
+            elif key == 27:
+                self.draw()
+                curses.curs_set(0)
+                return None
             elif key == ord('\n'):
                 break
 
         curses.curs_set(0)
-        txt = txt.split('.')[0]
         txt = txt.rstrip('_')
+        self.txt = txt
         return txt
 
 
-
 class Dialog:
 
     def set_selected(self, val):
         if self.selected >= 0:
             self.words[self.selected].selected = False
         self.selected = val
         if val >= 0:
@@ -311,15 +322,15 @@
         self.set_extension(extension)
 
     def _update_words(self):
         word_array = []
         for iy, row in enumerate(self.path_array[self.oy:self.oy+7]):
             wr = []
             for ix, p in enumerate(row):
-                wr.append(Word(self.y+1+iy, 1+ix*18, p, False))
+                wr.append(Word(self.y+1+iy, 1+ix*21, p, False))
             word_array.append(wr)
         self.word_array = word_array
 
     def set_extension(self, extension):
         self.extension = extension
         paths = [w.split('.')[0] for w in sorted(glob.glob(f'*.{extension}'))
                  if not w == 'pyniki.py']
@@ -327,15 +338,14 @@
         while paths:
             row, paths = paths[:4], paths[4:]
             path_array.append(row)
         self.path_array = path_array
         self.sy, self.sx, self.oy = -1, -1, 0
         self._update_words()
 
-
     def set_selected(self, sy, sx):
         if self.sy >= 0:
             self.word_array[self.sy-self.oy][self.sx].selected = False
         if sy < 0:
             self.draw()
             return
         self.sy, self.sx = sy, sx
@@ -378,15 +388,15 @@
                     self.set_selected(self.sy+1, min(self.sx, len(self.path_array[self.sy+1])-1))
             elif key == ord('\n'):
                 retval = self.path_array[self.sy][self.sx]
                 self.set_selected(-1, -1)
                 return retval
             elif key == 27:
                 self.set_selected(-1, -1)
-                return ''
+                return None
 
 
 
 class RobotDialog(Dialog):
 
     def __init__(self, y):
         self.y = y
@@ -765,48 +775,59 @@
             active_dialog = robot_dialog if active_dialog is field_dialog else field_dialog
             if active_dialog is robot_dialog:
                 file_dialog.set_extension('py')
             else:
                 file_dialog.set_extension('rob')
             draw()
         elif CMD == 'LOAD':
+            old_filename = active_dialog.filename.txt
             filename = active_dialog.filename.edit('')
+            if filename is None:
+                continue
             if not filename:
                 filename = file_dialog.run()
-            filename = filename[:8]
+                if filename is None:
+                    active_dialog.filename.txt = old_filename
+                    active_dialog.draw()
+                    continue
+                active_dialog.filename.txt = filename
+                active_dialog.draw()
             if active_dialog is robot_dialog:
                 filename = filename + '.py'
             else:
                 filename = filename + '.rob'
             if not os.path.exists(filename):
+                active_dialog.filename.txt = ''
                 continue
             if active_dialog is robot_dialog:
                 with open(filename, 'rt') as f:
                     program = f.read()
             else:
                 with open(filename, 'rb') as f:
                     field = pickle.load(f)
                     field.name = filename
-            active_dialog.filename.txt = filename
         elif CMD == 'SAVE':
             filename = active_dialog.filename.edit()
-            filename = filename[:8]
+            if filename is None:
+                continue
             if active_dialog is robot_dialog:
                 filename = filename + '.py'
             else:
                 filename = filename + '.rob'
             if active_dialog is robot_dialog:
                 with open(filename, 'wt') as f:
                     f.write(program)
             else:
                 with open(filename, 'wb') as f:
                     pickle.dump(field, f)
-            active_dialog.filename.txt = filename
+            file_dialog.set_extension(file_dialog.extension)
+            draw()
         elif CMD == 'EDIT':
             if active_dialog is robot_dialog:
+                _teardown()
                 p = subprocess.run(['micro', '-tabstospaces', 'true', '-filetype', 'python'],
                                    input=program.encode(),
                                    capture_output=True)
                 program = p.stdout.decode()
                 _setup()
                 draw()
             else:
@@ -820,13 +841,16 @@
         elif CMD == 'RUN':
             run_program()
             draw()
         elif CMD == 'QUIT':
             break
 
 def run():
+    path = pathlib.Path.home() / 'pyniki'
+    path.mkdir(exist_ok=True)
+    os.chdir(path)
     _setup()
     main_menu()
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `pyniki-0.0.1/LICENSE` & `pyniki-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyniki-0.0.1/pyproject.toml` & `pyniki-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyNIKI"
-version = "0.0.1"
+version = "0.0.2"
 description = "Classic Niki the robot in Python"
 readme = "README.md"
 license.file = "LICENSE"
 requires-python = ">=3.8"
 authors = [
     { name = "Stephan Rave", email = "stephan.rave@uni-muenster.de" },
 ]
```

### Comparing `pyniki-0.0.1/PKG-INFO` & `pyniki-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNIKI
-Version: 0.0.1
+Version: 0.0.2
 Summary: Classic Niki the robot in Python
 Project-URL: Homepage, https://github.com/sdrave/pyniki
 Author-email: Stephan Rave <stephan.rave@uni-muenster.de>
 Maintainer-email: Stephan Rave <stephan.rave@uni-muenster.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
```

