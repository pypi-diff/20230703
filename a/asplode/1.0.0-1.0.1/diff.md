# Comparing `tmp/asplode-1.0.0.tar.gz` & `tmp/asplode-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asplode-1.0.0.tar", last modified: Fri Jun 30 21:25:51 2023, max compression
+gzip compressed data, was "asplode-1.0.1.tar", last modified: Mon Jul  3 21:42:43 2023, max compression
```

## Comparing `asplode-1.0.0.tar` & `asplode-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brent      (502) staff       (20)        0 2023-06-30 21:25:51.294404 asplode-1.0.0/
--rw-r--r--   0 brent      (502) staff       (20)    11357 2021-07-09 18:47:25.000000 asplode-1.0.0/LICENSE
--rw-r--r--   0 brent      (502) staff       (20)      510 2023-06-30 21:25:51.294134 asplode-1.0.0/PKG-INFO
--rw-r--r--   0 brent      (502) staff       (20)      624 2023-06-30 20:55:30.000000 asplode-1.0.0/README.md
-drwxr-xr-x   0 brent      (502) staff       (20)        0 2023-06-30 21:25:51.293727 asplode-1.0.0/asplode.egg-info/
--rw-r--r--   0 brent      (502) staff       (20)      510 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/PKG-INFO
--rw-r--r--   0 brent      (502) staff       (20)      255 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/SOURCES.txt
--rw-r--r--   0 brent      (502) staff       (20)        1 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/dependency_links.txt
--rw-r--r--   0 brent      (502) staff       (20)       41 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/entry_points.txt
--rw-r--r--   0 brent      (502) staff       (20)        1 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/not-zip-safe
--rw-r--r--   0 brent      (502) staff       (20)        5 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/requires.txt
--rw-r--r--   0 brent      (502) staff       (20)        8 2023-06-30 21:25:51.000000 asplode-1.0.0/asplode.egg-info/top_level.txt
--rw-r--r--   0 brent      (502) staff       (20)     4122 2023-06-30 20:50:08.000000 asplode-1.0.0/asplode.py
--rw-r--r--   0 brent      (502) staff       (20)       38 2023-06-30 21:25:51.294493 asplode-1.0.0/setup.cfg
--rw-r--r--   0 brent      (502) staff       (20)      778 2023-06-30 21:24:57.000000 asplode-1.0.0/setup.py
+drwxr-xr-x   0 brent      (502) staff       (20)        0 2023-07-03 21:42:43.971954 asplode-1.0.1/
+-rw-r--r--   0 brent      (502) staff       (20)    11357 2021-07-09 18:47:25.000000 asplode-1.0.1/LICENSE
+-rw-r--r--   0 brent      (502) staff       (20)      510 2023-07-03 21:42:43.971660 asplode-1.0.1/PKG-INFO
+-rw-r--r--   0 brent      (502) staff       (20)      624 2023-06-30 20:55:30.000000 asplode-1.0.1/README.md
+drwxr-xr-x   0 brent      (502) staff       (20)        0 2023-07-03 21:42:43.971248 asplode-1.0.1/asplode.egg-info/
+-rw-r--r--   0 brent      (502) staff       (20)      510 2023-07-03 21:42:43.000000 asplode-1.0.1/asplode.egg-info/PKG-INFO
+-rw-r--r--   0 brent      (502) staff       (20)      255 2023-07-03 21:42:43.000000 asplode-1.0.1/asplode.egg-info/SOURCES.txt
+-rw-r--r--   0 brent      (502) staff       (20)        1 2023-07-03 21:42:43.000000 asplode-1.0.1/asplode.egg-info/dependency_links.txt
+-rw-r--r--   0 brent      (502) staff       (20)       41 2023-07-03 21:42:43.000000 asplode-1.0.1/asplode.egg-info/entry_points.txt
+-rw-r--r--   0 brent      (502) staff       (20)        1 2023-07-03 21:42:43.000000 asplode-1.0.1/asplode.egg-info/not-zip-safe
+-rw-r--r--   0 brent      (502) staff       (20)        5 2023-07-03 21:42:43.000000 asplode-1.0.1/asplode.egg-info/requires.txt
+-rw-r--r--   0 brent      (502) staff       (20)        8 2023-07-03 21:42:43.000000 asplode-1.0.1/asplode.egg-info/top_level.txt
+-rw-r--r--   0 brent      (502) staff       (20)     4127 2023-07-03 21:40:42.000000 asplode-1.0.1/asplode.py
+-rw-r--r--   0 brent      (502) staff       (20)       38 2023-07-03 21:42:43.972071 asplode-1.0.1/setup.cfg
+-rw-r--r--   0 brent      (502) staff       (20)      778 2023-07-03 21:41:25.000000 asplode-1.0.1/setup.py
```

### Comparing `asplode-1.0.0/LICENSE` & `asplode-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asplode-1.0.0/README.md` & `asplode-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `asplode-1.0.0/asplode.py` & `asplode-1.0.1/asplode.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,25 +87,25 @@
 
     try:
         extract_files = [f for f in list(extract_dir.glob("*")) if f != extract_dir]
         if len(extract_files) == 1:
             # If there's only one file/dir in the dir, move the file/dir back
             # one into the parent dir and remove the extract directory.  The
             # classic tar.gz -> dir and txt.gz -> file cases.
-            shutil.move(extract_files[0], str(start_dir))
+            shutil.move(str(extract_files[0]), str(start_dir))
             shutil.rmtree(extract_dir.name)
 
             # Set the name of the extracted dir for recursive decompression
             extract_dir = start_dir / Path(extract_files[0].name)
         else:
             # If there's more than one file in the dir, rename the extract dir
             # to the basename of the archive. The 'barfing files all over pwd'
             # case, the 'archive contains usr/bin and var/log/blah/blah and
             # etc' case.
-            shutil.move(extract_dir.name, basepath.name)
+            shutil.move(str(extract_dir), basepath.name)
 
             # Set the name of the extracted dir for recursive decompression
             extract_dir = basepath
     except shutil.Error as e:
         print(' Error arranging directories:')
         print(' ' + e)
         return
```

### Comparing `asplode-1.0.0/setup.py` & `asplode-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="asplode",
-    version="1.0.0",
+    version="1.0.1",
     description="Recursively decompress archives",
     long_description="Recursively decompress archives",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Utilities",
```

