# Comparing `tmp/wordflow-0.2.2.tar.gz` & `tmp/wordflow-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordflow-0.2.2.tar", max compression
+gzip compressed data, was "wordflow-0.2.4.tar", max compression
```

## Comparing `wordflow-0.2.2.tar` & `wordflow-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2733 2023-04-21 21:20:18.015509 wordflow-0.2.2/README.md
--rw-r--r--   0        0        0      682 2023-04-21 21:21:00.483244 wordflow-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 13:18:55.609572 wordflow-0.2.2/wordflow/__init__.py
--rw-r--r--   0        0        0      101 2023-04-21 13:58:45.274489 wordflow-0.2.2/wordflow/cli/count.py
--rw-r--r--   0        0        0     1138 2023-04-21 21:11:42.865172 wordflow-0.2.2/wordflow/cli/equal.py
--rw-r--r--   0        0        0      541 2023-04-21 16:04:45.838288 wordflow-0.2.2/wordflow/cli/frequency.py
--rw-r--r--   0        0        0      514 2023-04-21 16:04:13.879276 wordflow-0.2.2/wordflow/cli/length.py
--rw-r--r--   0        0        0     1299 2023-04-21 21:03:38.425773 wordflow-0.2.2/wordflow/cli/lessthan.py
--rw-r--r--   0        0        0      555 2023-04-21 16:02:22.444874 wordflow-0.2.2/wordflow/cli/match.py
--rw-r--r--   0        0        0      579 2023-04-21 18:14:10.862835 wordflow-0.2.2/wordflow/cli/max.py
--rw-r--r--   0        0        0      580 2023-04-21 18:14:01.345739 wordflow-0.2.2/wordflow/cli/min.py
--rw-r--r--   0        0        0      996 2023-04-21 16:11:10.563267 wordflow-0.2.2/wordflow/cli/order.py
--rw-r--r--   0        0        0      425 2023-04-21 16:03:46.266136 wordflow-0.2.2/wordflow/cli/pluck.py
--rw-r--r--   0        0        0      499 2023-04-21 21:06:30.615593 wordflow-0.2.2/wordflow/cli/put.py
--rw-r--r--   0        0        0       26 2023-04-21 13:46:51.770583 wordflow-0.2.2/wordflow/cli/reverse.py
--rw-r--r--   0        0        0      559 2023-04-21 20:41:40.966713 wordflow-0.2.2/wordflow/cli/unique.py
--rw-r--r--   0        0        0      787 2023-04-21 16:12:58.723877 wordflow-0.2.2/wordflow/pipe_guard.py
--rw-r--r--   0        0        0     3079 1970-01-01 00:00:00.000000 wordflow-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2733 2023-04-21 21:20:18.015509 wordflow-0.2.4/README.md
+-rw-r--r--   0        0        0      682 2023-07-03 00:51:17.689597 wordflow-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 13:18:55.609572 wordflow-0.2.4/wordflow/__init__.py
+-rw-r--r--   0        0        0      101 2023-04-21 13:58:45.274489 wordflow-0.2.4/wordflow/cli/count.py
+-rw-r--r--   0        0        0     1160 2023-04-22 03:06:44.049819 wordflow-0.2.4/wordflow/cli/equal.py
+-rw-r--r--   0        0        0      541 2023-04-21 16:04:45.838288 wordflow-0.2.4/wordflow/cli/frequency.py
+-rw-r--r--   0        0        0      514 2023-04-21 16:04:13.879276 wordflow-0.2.4/wordflow/cli/length.py
+-rw-r--r--   0        0        0     1321 2023-04-22 03:06:24.151336 wordflow-0.2.4/wordflow/cli/lessthan.py
+-rw-r--r--   0        0        0      555 2023-04-21 16:02:22.444874 wordflow-0.2.4/wordflow/cli/match.py
+-rw-r--r--   0        0        0      579 2023-04-21 18:14:10.862835 wordflow-0.2.4/wordflow/cli/max.py
+-rw-r--r--   0        0        0      580 2023-04-21 18:14:01.345739 wordflow-0.2.4/wordflow/cli/min.py
+-rw-r--r--   0        0        0      996 2023-04-21 16:11:10.563267 wordflow-0.2.4/wordflow/cli/order.py
+-rw-r--r--   0        0        0      425 2023-04-21 16:03:46.266136 wordflow-0.2.4/wordflow/cli/pluck.py
+-rw-r--r--   0        0        0      499 2023-04-21 21:06:30.615593 wordflow-0.2.4/wordflow/cli/put.py
+-rw-r--r--   0        0        0       26 2023-04-21 13:46:51.770583 wordflow-0.2.4/wordflow/cli/reverse.py
+-rw-r--r--   0        0        0      559 2023-04-21 20:41:40.966713 wordflow-0.2.4/wordflow/cli/unique.py
+-rw-r--r--   0        0        0      787 2023-04-21 16:12:58.723877 wordflow-0.2.4/wordflow/pipe_guard.py
+-rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 wordflow-0.2.4/PKG-INFO
```

### Comparing `wordflow-0.2.2/README.md` & `wordflow-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.2/pyproject.toml` & `wordflow-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "wordflow"
-version = "0.2.2"
+version = "0.2.4"
 description = ""
 authors = ["Chris Proctor <github.com@accounts.chrisproctor.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 wordfreq = "^3.0.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `wordflow-0.2.2/wordflow/cli/equal.py` & `wordflow-0.2.4/wordflow/cli/equal.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import sys
 from wordflow.pipe_guard import guard_pipe
 from argparse import ArgumentParser
 
 @guard_pipe
 def main():
     parser = ArgumentParser()
-    parser.add_argument('first', type=int, default=0)
-    parser.add_argument('second', type=int, default=1)
+    parser.add_argument('first', type=int, nargs='?', default=0)
+    parser.add_argument('second', type=int, nargs='?', default=1)
     arguments = parser.parse_args()
     for line in sys.stdin:
         tokens = line.split()
         try: 
             a, b = float(tokens[arguments.first]), float(tokens[arguments.second])
         except IndexError:
             raise Exception(
```

### Comparing `wordflow-0.2.2/wordflow/cli/frequency.py` & `wordflow-0.2.4/wordflow/cli/frequency.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.2/wordflow/cli/length.py` & `wordflow-0.2.4/wordflow/cli/length.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.2/wordflow/cli/lessthan.py` & `wordflow-0.2.4/wordflow/cli/lessthan.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import sys
 from wordflow.pipe_guard import guard_pipe
 from argparse import ArgumentParser
 
 @guard_pipe
 def main():
     parser = ArgumentParser()
-    parser.add_argument('first', type=int, default=0)
-    parser.add_argument('second', type=int, default=1)
+    parser.add_argument('first', type=int, nargs='?', default=0)
+    parser.add_argument('second', type=int, nargs='?', default=1)
     parser.add_argument('-e', '--equal', action='store_true')
     arguments = parser.parse_args()
     for line in sys.stdin:
         tokens = line.split()
         try: 
             a, b = float(tokens[arguments.first]), float(tokens[arguments.second])
         except IndexError:
```

### Comparing `wordflow-0.2.2/wordflow/cli/match.py` & `wordflow-0.2.4/wordflow/cli/match.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.2/wordflow/cli/max.py` & `wordflow-0.2.4/wordflow/cli/max.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.2/wordflow/cli/min.py` & `wordflow-0.2.4/wordflow/cli/min.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.2/wordflow/cli/order.py` & `wordflow-0.2.4/wordflow/cli/order.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.2/wordflow/cli/unique.py` & `wordflow-0.2.4/wordflow/cli/unique.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.2/wordflow/pipe_guard.py` & `wordflow-0.2.4/wordflow/pipe_guard.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.2/PKG-INFO` & `wordflow-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: wordflow
-Version: 0.2.2
+Version: 0.2.4
 Summary: 
 Author: Chris Proctor
 Author-email: github.com@accounts.chrisproctor.net
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: wordfreq (>=3.0.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 # WordFlow
 
 WordFlow provides several simplified command-line utilities meant to be
```

