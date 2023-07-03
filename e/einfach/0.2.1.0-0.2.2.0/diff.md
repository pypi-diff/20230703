# Comparing `tmp/einfach-0.2.1.0.tar.gz` & `tmp/einfach-0.2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einfach-0.2.1.0.tar", last modified: Mon Jul  3 14:13:41 2023, max compression
+gzip compressed data, was "einfach-0.2.2.0.tar", last modified: Mon Jul  3 16:41:09 2023, max compression
```

## Comparing `einfach-0.2.1.0.tar` & `einfach-0.2.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:13:41.190288 einfach-0.2.1.0/
--rw-rw-rw-   0        0        0     1144 2023-07-03 14:13:41.190288 einfach-0.2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-04-02 00:01:01.000000 einfach-0.2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 14:13:41.166279 einfach-0.2.1.0/einfach/
--rw-rw-rw-   0        0        0      156 2023-07-03 14:13:32.000000 einfach-0.2.1.0/einfach/__init__.py
--rw-rw-rw-   0        0        0      490 2023-07-03 14:12:37.000000 einfach-0.2.1.0/einfach/clip.py
--rw-rw-rw-   0        0        0      286 2023-07-03 14:12:37.000000 einfach-0.2.1.0/einfach/floatutils.py
--rw-rw-rw-   0        0        0     1688 2023-07-03 14:12:37.000000 einfach-0.2.1.0/einfach/pathdialog.py
--rw-rw-rw-   0        0        0     1480 2023-07-03 14:12:37.000000 einfach-0.2.1.0/einfach/termutils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:13:41.182272 einfach-0.2.1.0/einfach.egg-info/
--rw-rw-rw-   0        0        0     1144 2023-07-03 14:13:41.000000 einfach-0.2.1.0/einfach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-03 14:13:41.000000 einfach-0.2.1.0/einfach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:13:41.000000 einfach-0.2.1.0/einfach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 14:13:41.000000 einfach-0.2.1.0/einfach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:13:41.190288 einfach-0.2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1553 2023-07-03 14:12:37.000000 einfach-0.2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:41:09.145681 einfach-0.2.2.0/
+-rw-rw-rw-   0        0        0     1144 2023-07-03 16:41:09.145681 einfach-0.2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-04-02 00:01:01.000000 einfach-0.2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 16:41:09.113627 einfach-0.2.2.0/einfach/
+-rw-rw-rw-   0        0        0      156 2023-07-03 14:33:12.000000 einfach-0.2.2.0/einfach/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-07-03 14:12:37.000000 einfach-0.2.2.0/einfach/clip.py
+-rw-rw-rw-   0        0        0      286 2023-07-03 14:12:37.000000 einfach-0.2.2.0/einfach/floatutils.py
+-rw-rw-rw-   0        0        0     1688 2023-07-03 14:12:37.000000 einfach-0.2.2.0/einfach/pathdialog.py
+-rw-rw-rw-   0        0        0     1474 2023-07-03 14:32:54.000000 einfach-0.2.2.0/einfach/termutils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:41:09.137656 einfach-0.2.2.0/einfach.egg-info/
+-rw-rw-rw-   0        0        0     1144 2023-07-03 16:41:08.000000 einfach-0.2.2.0/einfach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-03 16:41:09.000000 einfach-0.2.2.0/einfach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 16:41:08.000000 einfach-0.2.2.0/einfach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 16:41:08.000000 einfach-0.2.2.0/einfach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 16:41:09.145681 einfach-0.2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-07-03 14:12:37.000000 einfach-0.2.2.0/setup.py
```

### Comparing `einfach-0.2.1.0/PKG-INFO` & `einfach-0.2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einfach
-Version: 0.2.1.0
+Version: 0.2.2.0
 Summary: A collection of useful code "snippets"
 Home-page: https://github.com/rotgruengelb/einfach
 Author: rotgruengelb (Daniel)
 Author-email: <code@rotgruengelb.net>
 License: MIT
 Project-URL: Source, https://github.com/rotgruengelb/einfach
 Project-URL: Issues, https://github.com/rotgruengelb/einfach/issues
```

### Comparing `einfach-0.2.1.0/einfach/pathdialog.py` & `einfach-0.2.2.0/einfach/pathdialog.py`

 * *Files identical despite different names*

### Comparing `einfach-0.2.1.0/einfach/termutils.py` & `einfach-0.2.2.0/einfach/termutils.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,29 +15,29 @@
     ```
     #### Args:
     ```py
         input_cbk: Callback function to be invoked when input is received.
     ```
     """
 
-    def __init__(self, input_callback: function, input_function: function = input, name: str = 'AsyncUserInput-thread'):
+    def __init__(self, input_callback, input_function = input, name: str = 'AsyncUserInput-thread'):
         self.input_callback = input_callback
         self.input_function = input_function
         self.name           = name
         self.paused         = False
         self.pause_cond     = threading.Condition(threading.Lock())
         super(AsyncUserInput, self).__init__(name=name)
         self.start()
 
     def run(self):
         while True:
             with self.pause_cond:
                 while self.paused:
                     self.pause_cond.wait()
-                self.input_callback(input())
+                self.input_callback(self.input_function())
 
     def pause(self):
         self.paused = True
         self.pause_cond.acquire()
         
     def resume(self):
         self.paused = False
```

### Comparing `einfach-0.2.1.0/einfach.egg-info/PKG-INFO` & `einfach-0.2.2.0/einfach.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einfach
-Version: 0.2.1.0
+Version: 0.2.2.0
 Summary: A collection of useful code "snippets"
 Home-page: https://github.com/rotgruengelb/einfach
 Author: rotgruengelb (Daniel)
 Author-email: <code@rotgruengelb.net>
 License: MIT
 Project-URL: Source, https://github.com/rotgruengelb/einfach
 Project-URL: Issues, https://github.com/rotgruengelb/einfach/issues
```

### Comparing `einfach-0.2.1.0/setup.py` & `einfach-0.2.2.0/setup.py`

 * *Files identical despite different names*

