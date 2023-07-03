# Comparing `tmp/sreddit-1.0.0.tar.gz` & `tmp/sreddit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sreddit-1.0.0.tar", last modified: Mon Jul  3 15:39:48 2023, max compression
+gzip compressed data, was "sreddit-1.0.1.tar", last modified: Mon Jul  3 15:49:01 2023, max compression
```

## Comparing `sreddit-1.0.0.tar` & `sreddit-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 15:39:48.563659 sreddit-1.0.0/
--rw-rw-rw-   0        0        0     1092 2023-07-02 18:37:29.000000 sreddit-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      501 2023-07-03 15:39:48.561621 sreddit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-07-03 15:39:36.000000 sreddit-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 15:39:48.564662 sreddit-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      799 2023-07-03 15:37:55.000000 sreddit-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:39:48.543245 sreddit-1.0.0/sreddit/
--rw-rw-rw-   0        0        0       74 2023-07-03 14:49:12.000000 sreddit-1.0.0/sreddit/__init__.py
--rw-rw-rw-   0        0        0     4262 2023-07-03 04:41:52.000000 sreddit-1.0.0/sreddit/srabstract.py
--rw-rw-rw-   0        0        0     3814 2023-07-03 05:08:04.000000 sreddit-1.0.0/sreddit/srbodies.py
--rw-rw-rw-   0        0        0     3707 2023-07-03 05:21:04.000000 sreddit-1.0.0/sreddit/srtitles.py
-drwxrwxrwx   0        0        0        0 2023-07-03 15:39:48.558333 sreddit-1.0.0/sreddit.egg-info/
--rw-rw-rw-   0        0        0      501 2023-07-03 15:39:48.000000 sreddit-1.0.0/sreddit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-03 15:39:48.000000 sreddit-1.0.0/sreddit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 15:39:48.000000 sreddit-1.0.0/sreddit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-03 15:39:48.000000 sreddit-1.0.0/sreddit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 15:39:48.000000 sreddit-1.0.0/sreddit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 15:49:01.087837 sreddit-1.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-07-02 18:37:29.000000 sreddit-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      501 2023-07-03 15:49:01.086815 sreddit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-07-03 15:39:36.000000 sreddit-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 15:49:01.087837 sreddit-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      786 2023-07-03 15:48:16.000000 sreddit-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:49:01.068091 sreddit-1.0.1/sreddit/
+-rw-rw-rw-   0        0        0       74 2023-07-03 14:49:12.000000 sreddit-1.0.1/sreddit/__init__.py
+-rw-rw-rw-   0        0        0     4262 2023-07-03 04:41:52.000000 sreddit-1.0.1/sreddit/srabstract.py
+-rw-rw-rw-   0        0        0     3814 2023-07-03 05:08:04.000000 sreddit-1.0.1/sreddit/srbodies.py
+-rw-rw-rw-   0        0        0     3707 2023-07-03 05:21:04.000000 sreddit-1.0.1/sreddit/srtitles.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:49:01.084772 sreddit-1.0.1/sreddit.egg-info/
+-rw-rw-rw-   0        0        0      501 2023-07-03 15:49:00.000000 sreddit-1.0.1/sreddit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-03 15:49:00.000000 sreddit-1.0.1/sreddit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 15:49:00.000000 sreddit-1.0.1/sreddit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-03 15:49:00.000000 sreddit-1.0.1/sreddit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 15:49:00.000000 sreddit-1.0.1/sreddit.egg-info/top_level.txt
```

### Comparing `sreddit-1.0.0/LICENSE` & `sreddit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sreddit-1.0.0/setup.py` & `sreddit-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sreddit",
-    version='1.0.0',
+    version='1.0.1',
     author="Mandy-cyber",
     author_email="",
     description='Web scraper for subreddits',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages=find_packages(),
     url="https://github.com/Mandy-cyber/sreddit",
-    install_requires=['selenium', 'get_chrome_driver', 'pysqlite3'],
+    install_requires=['selenium', 'get_chrome_driver'],
     keywords=['python', 'selenium', 'reddit', 'subreddit'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     python_requires = ">=3.6"
```

### Comparing `sreddit-1.0.0/sreddit/srabstract.py` & `sreddit-1.0.1/sreddit/srabstract.py`

 * *Files identical despite different names*

### Comparing `sreddit-1.0.0/sreddit/srbodies.py` & `sreddit-1.0.1/sreddit/srbodies.py`

 * *Files identical despite different names*

### Comparing `sreddit-1.0.0/sreddit/srtitles.py` & `sreddit-1.0.1/sreddit/srtitles.py`

 * *Files identical despite different names*

