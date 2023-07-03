# Comparing `tmp/bkapi-plugins-py-0.6281.tar.gz` & `tmp/bkapi-plugins-py-0.703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.6281.tar", last modified: Wed Jun 28 09:53:55 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.703.tar", last modified: Mon Jul  3 07:03:00 2023, max compression
```

## Comparing `bkapi-plugins-py-0.6281.tar` & `bkapi-plugins-py-0.703.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 09:53:55.542523 bkapi-plugins-py-0.6281/
--rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.6281/MANIFEST.in
--rw-rw-rw-   0        0        0      258 2023-06-28 09:53:55.543518 bkapi-plugins-py-0.6281/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-28 09:53:55.507783 bkapi-plugins-py-0.6281/bkapi_plugins/
-drwxrwxrwx   0        0        0        0 2023-06-28 09:53:55.524516 bkapi-plugins-py-0.6281/bkapi_plugins/files/
--rw-rw-rw-   0        0        0    36372 2023-06-28 08:17:43.000000 bkapi-plugins-py-0.6281/bkapi_plugins/files/influxdb-internals_rev1.json
--rw-rw-rw-   0        0        0    25365 2023-06-28 08:34:08.000000 bkapi-plugins-py-0.6281/bkapi_plugins/files/influxdb-metrics_rev1.json
--rw-rw-rw-   0        0        0    27326 2023-06-28 09:50:02.000000 bkapi-plugins-py-0.6281/bkapi_plugins/files/influxdb-oss-monitor-dashboard.json
-drwxrwxrwx   0        0        0        0 2023-06-28 09:53:55.541010 bkapi-plugins-py-0.6281/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      258 2023-06-28 09:53:55.000000 bkapi-plugins-py-0.6281/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-06-28 09:53:55.000000 bkapi-plugins-py-0.6281/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 09:53:55.000000 bkapi-plugins-py-0.6281/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 09:53:55.000000 bkapi-plugins-py-0.6281/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 09:53:55.545999 bkapi-plugins-py-0.6281/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-06-28 09:53:46.000000 bkapi-plugins-py-0.6281/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 07:03:00.587873 bkapi-plugins-py-0.703/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.703/MANIFEST.in
+-rw-rw-rw-   0        0        0      257 2023-07-03 07:03:00.587873 bkapi-plugins-py-0.703/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-03 07:03:00.575761 bkapi-plugins-py-0.703/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-07-03 07:03:00.580765 bkapi-plugins-py-0.703/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0      438 2023-07-03 07:01:21.000000 bkapi-plugins-py-0.703/bkapi_plugins/files/process.sh
+drwxrwxrwx   0        0        0        0 2023-07-03 07:03:00.586872 bkapi-plugins-py-0.703/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-07-03 07:03:00.000000 bkapi-plugins-py-0.703/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-07-03 07:03:00.000000 bkapi-plugins-py-0.703/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 07:03:00.000000 bkapi-plugins-py-0.703/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 07:03:00.000000 bkapi-plugins-py-0.703/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 07:03:00.589873 bkapi-plugins-py-0.703/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-07-03 07:02:53.000000 bkapi-plugins-py-0.703/setup.py
```

### Comparing `bkapi-plugins-py-0.6281/setup.py` & `bkapi-plugins-py-0.703/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
     name='bkapi-plugins-py', # 包的名字
-    version='0.6281', # 版本号每次打包完要改一下
+    version='0.703', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

