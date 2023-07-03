# Comparing `tmp/testlibcreation-0.0.1.tar.gz` & `tmp/testlibcreation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testlibcreation-0.0.1.tar", last modified: Sat May 27 14:31:51 2023, max compression
+gzip compressed data, was "testlibcreation-0.0.2.tar", last modified: Mon Jul  3 14:32:56 2023, max compression
```

## Comparing `testlibcreation-0.0.1.tar` & `testlibcreation-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:31:51.939160 testlibcreation-0.0.1/
--rw-rw-r--   0 sergey    (1000) sergey    (1000)    35149 2023-05-27 14:06:48.000000 testlibcreation-0.0.1/LICENSE
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      482 2023-05-27 14:31:51.939160 testlibcreation-0.0.1/PKG-INFO
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       17 2023-05-27 14:06:48.000000 testlibcreation-0.0.1/README.md
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       38 2023-05-27 14:31:51.939160 testlibcreation-0.0.1/setup.cfg
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      695 2023-05-27 14:29:16.000000 testlibcreation-0.0.1/setup.py
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:31:51.935160 testlibcreation-0.0.1/testlibcreation/
--rw-rw-r--   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:08:35.000000 testlibcreation-0.0.1/testlibcreation/__init__.py
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      225 2023-05-27 14:18:25.000000 testlibcreation-0.0.1/testlibcreation/testlibcreation.py
-drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 14:31:51.939160 testlibcreation-0.0.1/testlibcreation.egg-info/
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      482 2023-05-27 14:31:51.000000 testlibcreation-0.0.1/testlibcreation.egg-info/PKG-INFO
--rw-rw-r--   0 sergey    (1000) sergey    (1000)      245 2023-05-27 14:31:51.000000 testlibcreation-0.0.1/testlibcreation.egg-info/SOURCES.txt
--rw-rw-r--   0 sergey    (1000) sergey    (1000)        1 2023-05-27 14:31:51.000000 testlibcreation-0.0.1/testlibcreation.egg-info/dependency_links.txt
--rw-rw-r--   0 sergey    (1000) sergey    (1000)       16 2023-05-27 14:31:51.000000 testlibcreation-0.0.1/testlibcreation.egg-info/top_level.txt
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-03 14:32:56.954229 testlibcreation-0.0.2/
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)    35149 2023-07-03 13:37:56.000000 testlibcreation-0.0.2/LICENSE
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      482 2023-07-03 14:32:56.954229 testlibcreation-0.0.2/PKG-INFO
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       17 2023-07-03 13:37:56.000000 testlibcreation-0.0.2/README.md
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       38 2023-07-03 14:32:56.954229 testlibcreation-0.0.2/setup.cfg
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      695 2023-07-03 13:55:29.000000 testlibcreation-0.0.2/setup.py
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-03 14:32:56.954229 testlibcreation-0.0.2/testlibcreation/
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)        0 2023-07-03 13:37:56.000000 testlibcreation-0.0.2/testlibcreation/__init__.py
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      190 2023-07-03 13:53:14.000000 testlibcreation-0.0.2/testlibcreation/testlibcreation.py
+drwxrwxr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-03 14:32:56.954229 testlibcreation-0.0.2/testlibcreation.egg-info/
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      482 2023-07-03 14:32:56.000000 testlibcreation-0.0.2/testlibcreation.egg-info/PKG-INFO
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)      245 2023-07-03 14:32:56.000000 testlibcreation-0.0.2/testlibcreation.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)        1 2023-07-03 14:32:56.000000 testlibcreation-0.0.2/testlibcreation.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergey    (1000) sergey    (1000)       16 2023-07-03 14:32:56.000000 testlibcreation-0.0.2/testlibcreation.egg-info/top_level.txt
```

### Comparing `testlibcreation-0.0.1/LICENSE` & `testlibcreation-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `testlibcreation-0.0.1/setup.py` & `testlibcreation-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = []
 
 setup(
     name="testlibcreation",
-    version="0.0.1",
+    version="0.0.2",
     author="Sergey Zamyatin",
     author_email="sergey.zamyatin.01@list.ru",
     description="A package to convert your Jupyter Notebook",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/SergeyZamyatin1/testlibcreation",
     packages=find_packages(),
```

