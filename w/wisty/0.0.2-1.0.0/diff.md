# Comparing `tmp/wisty-0.0.2.tar.gz` & `tmp/wisty-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wisty-0.0.2.tar", last modified: Fri Dec 25 19:14:08 2020, max compression
+gzip compressed data, was "wisty-1.0.0.tar", last modified: Mon Jul  3 00:28:27 2023, max compression
```

## Comparing `wisty-0.0.2.tar` & `wisty-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-25 19:14:08.000000 wisty-0.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-25 19:14:08.000000 wisty-0.0.2/wisty.egg-info/
--rw-r--r--   0 root         (0) root         (0)      212 2020-12-25 19:14:08.000000 wisty-0.0.2/wisty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1761 2020-12-25 19:14:08.000000 wisty-0.0.2/wisty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2020-12-25 19:14:08.000000 wisty-0.0.2/wisty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-12-25 19:14:08.000000 wisty-0.0.2/wisty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2020-12-25 19:14:08.000000 wisty-0.0.2/wisty.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       43 2020-12-25 19:14:08.000000 wisty-0.0.2/wisty.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)     1036 2020-12-25 19:13:47.000000 wisty-0.0.2/setup.py
--rw-r--r--   0 root         (0) root         (0)     1761 2020-12-25 19:14:08.000000 wisty-0.0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      869 2020-12-25 19:07:08.000000 wisty-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-25 19:14:08.000000 wisty-0.0.2/wisty/
--rwxrwxr-x   0 root         (0) root         (0)     4269 2020-12-25 19:09:46.000000 wisty-0.0.2/wisty/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-12-25 19:14:08.000000 wisty-0.0.2/setup.cfg
+drwxr-xr-x   0 df-4       (501) staff       (20)        0 2023-07-03 00:28:27.222799 wisty-1.0.0/
+-rw-r--r--   0 df-4       (501) staff       (20)     1070 2023-07-02 23:06:38.000000 wisty-1.0.0/LICENSE
+-rw-r--r--   0 df-4       (501) staff       (20)     1520 2023-07-03 00:28:27.222663 wisty-1.0.0/PKG-INFO
+-rw-r--r--   0 df-4       (501) staff       (20)      948 2023-07-02 23:06:38.000000 wisty-1.0.0/README.md
+-rw-r--r--   0 df-4       (501) staff       (20)       38 2023-07-03 00:28:27.222861 wisty-1.0.0/setup.cfg
+-rw-r--r--   0 df-4       (501) staff       (20)     1022 2023-07-03 00:23:25.000000 wisty-1.0.0/setup.py
+drwxr-xr-x   0 df-4       (501) staff       (20)        0 2023-07-03 00:28:27.221672 wisty-1.0.0/wisty/
+-rwxr-xr-x   0 df-4       (501) staff       (20)     3380 2023-07-03 00:22:39.000000 wisty-1.0.0/wisty/__init__.py
+drwxr-xr-x   0 df-4       (501) staff       (20)        0 2023-07-03 00:28:27.222492 wisty-1.0.0/wisty.egg-info/
+-rw-r--r--   0 df-4       (501) staff       (20)     1520 2023-07-03 00:28:27.000000 wisty-1.0.0/wisty.egg-info/PKG-INFO
+-rw-r--r--   0 df-4       (501) staff       (20)      220 2023-07-03 00:28:27.000000 wisty-1.0.0/wisty.egg-info/SOURCES.txt
+-rw-r--r--   0 df-4       (501) staff       (20)        1 2023-07-03 00:28:27.000000 wisty-1.0.0/wisty.egg-info/dependency_links.txt
+-rw-r--r--   0 df-4       (501) staff       (20)       37 2023-07-03 00:28:27.000000 wisty-1.0.0/wisty.egg-info/entry_points.txt
+-rw-r--r--   0 df-4       (501) staff       (20)       43 2023-07-03 00:28:27.000000 wisty-1.0.0/wisty.egg-info/requires.txt
+-rw-r--r--   0 df-4       (501) staff       (20)        6 2023-07-03 00:28:27.000000 wisty-1.0.0/wisty.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wisty-0.0.2/setup.py` & `wisty-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,32 +4,30 @@
 current_dir = path.abspath(path.dirname(__file__))
 
 with open(path.join(current_dir, "README.md"), "r") as f:
     readme = f.read()
 
 setup(
     name="wisty",
-    version="0.0.2",
+    version="1.0.0",
     url="https://github.com/knowbee/wisty.git",
     author="Igwaneza Bruce",
     author_email="knowbeeinc@gmail.com",
     description="A fast minimal command line tool to download videos hosted on wistia with video id",
     long_description=readme,
     long_description_content_type="text/markdown",
     platforms="any",
     python_requires=">=3.6",
     packages=["wisty"],
     install_requires=[
         "click == 7.1.2",
         "requests == 2.23.0",
         "tqdm==4.54.1",
     ],
-    entry_points={
-        "console_scripts": ['wisty = wisty:main']
-    },
+    entry_points={"console_scripts": ["wisty = wisty:main"]},
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
     ],
```

### Comparing `wisty-0.0.2/README.md` & `wisty-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # wisty
 
+[![Downloads](https://pepy.tech/badge/wisty)](https://pepy.tech/project/wisty)
 [![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=102)](https://github.com/ellerbrock/open-source-badge/)
 [![Open Source Love](https://badges.frapsoft.com/os/mit/mit.svg?v=102)](https://github.com/ellerbrock/open-source-badge/)
 
 A fast minimal command line tool to download videos hosted on wistia with video id.
 
 ## Preview
```

