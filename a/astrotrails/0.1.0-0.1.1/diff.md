# Comparing `tmp/astrotrails-0.1.0-py3.10.egg` & `tmp/astrotrails-0.1.1-py3.10.egg`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 6212 bytes, number of entries: 11
--rw-rw-r--  2.0 unx     1098 b- defN 23-Jul-03 00:55 EGG-INFO/PKG-INFO
--rw-rw-r--  2.0 unx      328 b- defN 23-Jul-03 00:55 EGG-INFO/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-03 00:55 EGG-INFO/dependency_links.txt
--rw-rw-r--  2.0 unx       58 b- defN 23-Jul-03 00:55 EGG-INFO/entry_points.txt
+-rw-rw-r--  2.0 unx     1099 b- defN 23-Jul-03 01:36 EGG-INFO/PKG-INFO
+-rw-rw-r--  2.0 unx      328 b- defN 23-Jul-03 01:36 EGG-INFO/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-03 01:36 EGG-INFO/dependency_links.txt
+-rw-rw-r--  2.0 unx       58 b- defN 23-Jul-03 01:36 EGG-INFO/entry_points.txt
 -rw-rw-r--  2.0 unx        1 b- defN 23-Jul-03 00:25 EGG-INFO/not-zip-safe
--rw-rw-r--  2.0 unx       29 b- defN 23-Jul-03 00:55 EGG-INFO/requires.txt
--rw-rw-r--  2.0 unx       12 b- defN 23-Jul-03 00:55 EGG-INFO/top_level.txt
+-rw-rw-r--  2.0 unx       29 b- defN 23-Jul-03 01:36 EGG-INFO/requires.txt
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jul-03 01:36 EGG-INFO/top_level.txt
 -rw-rw-r--  2.0 unx     2595 b- defN 23-Jul-03 00:55 astrotrails/__init__.py
 -rw-rw-r--  2.0 unx     1940 b- defN 23-Jul-03 00:46 astrotrails/command_line.py
--rw-rw-r--  2.0 unx     2908 b- defN 23-Jul-03 00:55 astrotrails/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--  2.0 unx     1315 b- defN 23-Jul-03 00:55 astrotrails/__pycache__/command_line.cpython-310.pyc
-11 files, 10285 bytes uncompressed, 4744 bytes compressed:  53.9%
+-rw-rw-r--  2.0 unx     2908 b- defN 23-Jul-03 01:36 astrotrails/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--  2.0 unx     1315 b- defN 23-Jul-03 01:36 astrotrails/__pycache__/command_line.cpython-310.pyc
+11 files, 10286 bytes uncompressed, 4744 bytes compressed:  53.9%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: astrotrails
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool to generate startrails images by stacking consecutive starimages in jpeg format. Also, astrotrails can create a timelapse video.
 Home-page: https://github.com/theogatsios/astrotrails
 Author: Theo Gatsios
 Author-email: theogat@protonmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-#Astrotrails
+# Astrotrails
 Tool to generate startrails images by stacking consecutive acquisition in jpeg format. It can also generate timelapse videos.
 
 ## Setup and installation
 
 ```bash
 pip install astrotrails
 ```
```

