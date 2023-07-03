# Comparing `tmp/einfach-0.2.0.0.tar.gz` & `tmp/einfach-0.2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einfach-0.2.0.0.tar", last modified: Mon Jul  3 13:57:50 2023, max compression
+gzip compressed data, was "einfach-0.2.1.0.tar", last modified: Mon Jul  3 14:13:41 2023, max compression
```

## Comparing `einfach-0.2.0.0.tar` & `einfach-0.2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 13:57:50.662972 einfach-0.2.0.0/
--rw-rw-rw-   0        0        0     1144 2023-07-03 13:57:50.662972 einfach-0.2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-04-02 00:01:01.000000 einfach-0.2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 13:57:50.630982 einfach-0.2.0.0/einfach/
--rw-rw-rw-   0        0        0      156 2023-07-03 13:38:13.000000 einfach-0.2.0.0/einfach/__init__.py
--rw-rw-rw-   0        0        0      490 2023-07-03 13:11:00.000000 einfach-0.2.0.0/einfach/clip.py
--rw-rw-rw-   0        0        0      286 2023-07-03 13:29:22.000000 einfach-0.2.0.0/einfach/floatutils.py
--rw-rw-rw-   0        0        0     1690 2023-07-03 13:29:04.000000 einfach-0.2.0.0/einfach/pathdialog.py
--rw-rw-rw-   0        0        0     1480 2023-07-03 13:27:32.000000 einfach-0.2.0.0/einfach/termutils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 13:57:50.654975 einfach-0.2.0.0/einfach.egg-info/
--rw-rw-rw-   0        0        0     1144 2023-07-03 13:57:50.000000 einfach-0.2.0.0/einfach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-03 13:57:50.000000 einfach-0.2.0.0/einfach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 13:57:50.000000 einfach-0.2.0.0/einfach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 13:57:50.000000 einfach-0.2.0.0/einfach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 13:57:50.662972 einfach-0.2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1553 2023-07-03 13:57:22.000000 einfach-0.2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:13:41.190288 einfach-0.2.1.0/
+-rw-rw-rw-   0        0        0     1144 2023-07-03 14:13:41.190288 einfach-0.2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-04-02 00:01:01.000000 einfach-0.2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 14:13:41.166279 einfach-0.2.1.0/einfach/
+-rw-rw-rw-   0        0        0      156 2023-07-03 14:13:32.000000 einfach-0.2.1.0/einfach/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-07-03 14:12:37.000000 einfach-0.2.1.0/einfach/clip.py
+-rw-rw-rw-   0        0        0      286 2023-07-03 14:12:37.000000 einfach-0.2.1.0/einfach/floatutils.py
+-rw-rw-rw-   0        0        0     1688 2023-07-03 14:12:37.000000 einfach-0.2.1.0/einfach/pathdialog.py
+-rw-rw-rw-   0        0        0     1480 2023-07-03 14:12:37.000000 einfach-0.2.1.0/einfach/termutils.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:13:41.182272 einfach-0.2.1.0/einfach.egg-info/
+-rw-rw-rw-   0        0        0     1144 2023-07-03 14:13:41.000000 einfach-0.2.1.0/einfach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-03 14:13:41.000000 einfach-0.2.1.0/einfach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 14:13:41.000000 einfach-0.2.1.0/einfach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 14:13:41.000000 einfach-0.2.1.0/einfach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 14:13:41.190288 einfach-0.2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-07-03 14:12:37.000000 einfach-0.2.1.0/setup.py
```

### Comparing `einfach-0.2.0.0/PKG-INFO` & `einfach-0.2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einfach
-Version: 0.2.0.0
+Version: 0.2.1.0
 Summary: A collection of useful code "snippets"
 Home-page: https://github.com/rotgruengelb/einfach
 Author: rotgruengelb (Daniel)
 Author-email: <code@rotgruengelb.net>
 License: MIT
 Project-URL: Source, https://github.com/rotgruengelb/einfach
 Project-URL: Issues, https://github.com/rotgruengelb/einfach/issues
```

### Comparing `einfach-0.2.0.0/einfach/pathdialog.py` & `einfach-0.2.1.0/einfach/pathdialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,14 @@
         elif mode == "file_names":
             file_path = filedialog.askopenfilenames(**filedialogargs); return file_path
         else: raise ValueError("mode was not 'file', 'file_name', 'files' or 'file_names'!")
     except Exception as e:
         raise e
 
 
-def open_dir(**filedialogargs):
+def open_dir(**dirdialogargs):
     root = tk.Tk()
     root.withdraw()
     try:
-        dir_path = filedialog.askdirectory(**filedialogargs); return dir_path
+        dir_path = filedialog.askdirectory(**dirdialogargs); return dir_path
     except Exception as e:
         raise e
```

### Comparing `einfach-0.2.0.0/einfach/termutils.py` & `einfach-0.2.1.0/einfach/termutils.py`

 * *Files identical despite different names*

### Comparing `einfach-0.2.0.0/einfach.egg-info/PKG-INFO` & `einfach-0.2.1.0/einfach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einfach
-Version: 0.2.0.0
+Version: 0.2.1.0
 Summary: A collection of useful code "snippets"
 Home-page: https://github.com/rotgruengelb/einfach
 Author: rotgruengelb (Daniel)
 Author-email: <code@rotgruengelb.net>
 License: MIT
 Project-URL: Source, https://github.com/rotgruengelb/einfach
 Project-URL: Issues, https://github.com/rotgruengelb/einfach/issues
```

### Comparing `einfach-0.2.0.0/setup.py` & `einfach-0.2.1.0/setup.py`

 * *Files identical despite different names*

