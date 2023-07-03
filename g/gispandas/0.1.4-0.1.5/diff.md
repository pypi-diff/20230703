# Comparing `tmp/gispandas-0.1.4.tar.gz` & `tmp/gispandas-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gispandas-0.1.4.tar", last modified: Thu Jun 29 09:28:25 2023, max compression
+gzip compressed data, was "gispandas-0.1.5.tar", last modified: Mon Jul  3 09:22:47 2023, max compression
```

## Comparing `gispandas-0.1.4.tar` & `gispandas-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 09:28:25.067198 gispandas-0.1.4/
--rw-rw-rw-   0        0        0      236 2023-06-29 09:28:25.065196 gispandas-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-06-29 09:25:50.000000 gispandas-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 09:28:25.059181 gispandas-0.1.4/gispandas/
--rw-rw-rw-   0        0        0        0 2023-06-29 07:49:45.000000 gispandas-0.1.4/gispandas/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-06-29 06:54:45.000000 gispandas-0.1.4/gispandas/gispandas.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:28:25.064199 gispandas-0.1.4/gispandas.egg-info/
--rw-rw-rw-   0        0        0      236 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 09:28:25.067198 gispandas-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-06-29 09:27:27.000000 gispandas-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:22:47.323130 gispandas-0.1.5/
+-rw-rw-rw-   0        0        0     1026 2023-07-03 09:22:47.322132 gispandas-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-06-29 09:25:50.000000 gispandas-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 09:22:47.313157 gispandas-0.1.5/gispandas/
+-rw-rw-rw-   0        0        0        0 2023-06-29 07:49:45.000000 gispandas-0.1.5/gispandas/__init__.py
+-rw-rw-rw-   0        0        0     2652 2023-06-29 06:54:45.000000 gispandas-0.1.5/gispandas/gispandas.py
+drwxrwxrwx   0        0        0        0 2023-07-03 09:22:47.321135 gispandas-0.1.5/gispandas.egg-info/
+-rw-rw-rw-   0        0        0     1026 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-07-03 09:22:47.000000 gispandas-0.1.5/gispandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 09:22:47.323130 gispandas-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-07-03 09:21:06.000000 gispandas-0.1.5/setup.py
```

### Comparing `gispandas-0.1.4/README.md` & `gispandas-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gispandas-0.1.4/gispandas/gispandas.py` & `gispandas-0.1.5/gispandas/gispandas.py`

 * *Files identical despite different names*

### Comparing `gispandas-0.1.4/setup.py` & `gispandas-0.1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup, find_packages
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 filepath = path.join(this_directory, 'README.md')
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 setup(
     name='gispandas',  # package name
     version=VERSION,  # package version
     author="HMX",
     author_email="kzdhb8023@163.com",
     description='gispandas',  # package description
     packages=find_packages(),
     url="https://github.com/mxhou/gispandas/",
     zip_safe=False,
     # What packages are required for this module to be executed?
     REQUIRED = ['geopandas', 'numpy','json','rasterio','rasterstats'],
     license='MIT',
     python_requires=">=3.6",
     keywords=['gis','geo','tif','json'],
-    data_files=[filepath]
+    data_files=[filepath],
+    long_description=open(filepath, encoding='utf-8').read(),
+    long_description_content_type='text/markdown'
 )
```

