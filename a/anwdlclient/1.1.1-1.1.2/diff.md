# Comparing `tmp/anwdlclient-1.1.1.tar.gz` & `tmp/anwdlclient-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anwdlclient-1.1.1.tar", last modified: Mon Jul  3 14:46:06 2023, max compression
+gzip compressed data, was "anwdlclient-1.1.2.tar", last modified: Mon Jul  3 16:05:24 2023, max compression
```

## Comparing `anwdlclient-1.1.1.tar` & `anwdlclient-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.619700 anwdlclient-1.1.1/
--rw-r--r--   0 user      (1001) user      (1001)     1150 2023-05-17 20:18:52.000000 anwdlclient-1.1.1/CONTRIBUTING
--rwxrwxrwx   0 user      (1001) user      (1001)    35129 2022-12-14 12:17:41.000000 anwdlclient-1.1.1/LICENSE
--rw-r--r--   0 user      (1001) user      (1001)      204 2023-07-03 14:12:19.000000 anwdlclient-1.1.1/MANIFEST.in
--rw-r--r--   0 user      (1001) user      (1001)    43945 2023-07-03 14:46:06.619700 anwdlclient-1.1.1/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     2584 2023-07-03 14:32:39.000000 anwdlclient-1.1.1/README.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.616700 anwdlclient-1.1.1/anwdlclient/
--rw-r--r--   0 user      (1001) user      (1001)       27 2023-07-03 14:45:25.000000 anwdlclient-1.1.1/anwdlclient/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)    42965 2023-07-03 09:54:55.000000 anwdlclient-1.1.1/anwdlclient/cli.py
--rw-r--r--   0 user      (1001) user      (1001)     1216 2023-05-30 16:26:10.000000 anwdlclient-1.1.1/anwdlclient/config.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.618699 anwdlclient-1.1.1/anwdlclient/core/
--rw-r--r--   0 user      (1001) user      (1001)        0 2023-04-10 17:55:16.000000 anwdlclient-1.1.1/anwdlclient/core/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     7119 2023-06-04 18:55:02.000000 anwdlclient-1.1.1/anwdlclient/core/client.py
--rwxrwxrwx   0 user      (1001) user      (1001)     7935 2023-05-16 08:04:03.000000 anwdlclient-1.1.1/anwdlclient/core/crypto.py
--rwxrwxrwx   0 user      (1001) user      (1001)     5807 2023-05-16 20:10:18.000000 anwdlclient-1.1.1/anwdlclient/core/sanitize.py
--rw-r--r--   0 user      (1001) user      (1001)     1182 2023-06-02 14:13:15.000000 anwdlclient-1.1.1/anwdlclient/core/util.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.618699 anwdlclient-1.1.1/anwdlclient/tools/
--rw-r--r--   0 user      (1001) user      (1001)        0 2023-04-22 13:25:26.000000 anwdlclient-1.1.1/anwdlclient/tools/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     2966 2023-06-11 11:17:13.000000 anwdlclient-1.1.1/anwdlclient/tools/accesstk.py
--rw-r--r--   0 user      (1001) user      (1001)     7096 2023-06-11 17:18:30.000000 anwdlclient-1.1.1/anwdlclient/tools/credentials.py
--rwxr-xr-x   0 user      (1001) user      (1001)      217 2023-07-03 12:51:38.000000 anwdlclient-1.1.1/anwdlclient-uninstall
--rw-r--r--   0 user      (1001) user      (1001)      232 2023-06-26 21:22:50.000000 anwdlclient-1.1.1/anwdlclient-uninstall.bat
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.617699 anwdlclient-1.1.1/anwdlclient.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)    43945 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)      643 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) user      (1001)        1 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) user      (1001)       70 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/entry_points.txt
--rw-r--r--   0 user      (1001) user      (1001)       29 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/requires.txt
--rw-r--r--   0 user      (1001) user      (1001)       12 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) user      (1001)     1033 2023-07-03 14:45:17.000000 anwdlclient-1.1.1/pyproject.toml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.619700 anwdlclient-1.1.1/resources/
--rw-r--r--   0 user      (1001) user      (1001)      668 2023-05-30 08:48:18.000000 anwdlclient-1.1.1/resources/config.yaml
--rw-r--r--   0 user      (1001) user      (1001)       38 2023-07-03 14:46:06.619700 anwdlclient-1.1.1/setup.cfg
--rw-r--r--   0 user      (1001) user      (1001)     3079 2023-07-03 14:45:05.000000 anwdlclient-1.1.1/setup.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 16:05:24.482757 anwdlclient-1.1.2/
+-rw-r--r--   0 user      (1001) user      (1001)     1150 2023-05-17 20:18:52.000000 anwdlclient-1.1.2/CONTRIBUTING
+-rwxrwxrwx   0 user      (1001) user      (1001)    35129 2022-12-14 12:17:41.000000 anwdlclient-1.1.2/LICENSE
+-rw-r--r--   0 user      (1001) user      (1001)      204 2023-07-03 14:12:19.000000 anwdlclient-1.1.2/MANIFEST.in
+-rw-r--r--   0 user      (1001) user      (1001)      622 2023-07-03 16:05:24.481757 anwdlclient-1.1.2/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     2584 2023-07-03 14:55:06.000000 anwdlclient-1.1.2/README.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 16:05:24.479757 anwdlclient-1.1.2/anwdlclient/
+-rw-r--r--   0 user      (1001) user      (1001)       27 2023-07-03 16:04:30.000000 anwdlclient-1.1.2/anwdlclient/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)    42965 2023-07-03 09:54:55.000000 anwdlclient-1.1.2/anwdlclient/cli.py
+-rw-r--r--   0 user      (1001) user      (1001)     1216 2023-05-30 16:26:10.000000 anwdlclient-1.1.2/anwdlclient/config.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 16:05:24.481757 anwdlclient-1.1.2/anwdlclient/core/
+-rw-r--r--   0 user      (1001) user      (1001)        0 2023-04-10 17:55:16.000000 anwdlclient-1.1.2/anwdlclient/core/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     7119 2023-06-04 18:55:02.000000 anwdlclient-1.1.2/anwdlclient/core/client.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     7935 2023-05-16 08:04:03.000000 anwdlclient-1.1.2/anwdlclient/core/crypto.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     5807 2023-05-16 20:10:18.000000 anwdlclient-1.1.2/anwdlclient/core/sanitize.py
+-rw-r--r--   0 user      (1001) user      (1001)     1182 2023-06-02 14:13:15.000000 anwdlclient-1.1.2/anwdlclient/core/util.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 16:05:24.481757 anwdlclient-1.1.2/anwdlclient/tools/
+-rw-r--r--   0 user      (1001) user      (1001)        0 2023-04-22 13:25:26.000000 anwdlclient-1.1.2/anwdlclient/tools/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     2966 2023-06-11 11:17:13.000000 anwdlclient-1.1.2/anwdlclient/tools/accesstk.py
+-rw-r--r--   0 user      (1001) user      (1001)     7096 2023-06-11 17:18:30.000000 anwdlclient-1.1.2/anwdlclient/tools/credentials.py
+-rwxr-xr-x   0 user      (1001) user      (1001)      217 2023-07-03 12:51:38.000000 anwdlclient-1.1.2/anwdlclient-uninstall
+-rw-r--r--   0 user      (1001) user      (1001)      232 2023-06-26 21:22:50.000000 anwdlclient-1.1.2/anwdlclient-uninstall.bat
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 16:05:24.480757 anwdlclient-1.1.2/anwdlclient.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)      622 2023-07-03 16:05:24.000000 anwdlclient-1.1.2/anwdlclient.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)      628 2023-07-03 16:05:24.000000 anwdlclient-1.1.2/anwdlclient.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) user      (1001)        1 2023-07-03 16:05:24.000000 anwdlclient-1.1.2/anwdlclient.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) user      (1001)       70 2023-07-03 16:05:24.000000 anwdlclient-1.1.2/anwdlclient.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1001) user      (1001)       29 2023-07-03 16:05:24.000000 anwdlclient-1.1.2/anwdlclient.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) user      (1001)       12 2023-07-03 16:05:24.000000 anwdlclient-1.1.2/anwdlclient.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 16:05:24.481757 anwdlclient-1.1.2/resources/
+-rw-r--r--   0 user      (1001) user      (1001)      668 2023-05-30 08:48:18.000000 anwdlclient-1.1.2/resources/config.yaml
+-rw-r--r--   0 user      (1001) user      (1001)       38 2023-07-03 16:05:24.482757 anwdlclient-1.1.2/setup.cfg
+-rw-r--r--   0 user      (1001) user      (1001)     3189 2023-07-03 16:04:06.000000 anwdlclient-1.1.2/setup.py
```

### Comparing `anwdlclient-1.1.1/CONTRIBUTING` & `anwdlclient-1.1.2/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/LICENSE` & `anwdlclient-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/README.md` & `anwdlclient-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 Install it with pip (linux):
 ```
 $ pip install anwdlclient
 ```
 
 On windows : 
 ```
-$ py -m pip install anwdlserver
+$ py -m pip install anwdlclient
 ```
 
 ### Source installation
 
 Clone the client source code repository : 
 ```
 $ git clone https://github.com/the-anweddol-project/Anweddol-client.git
```

### Comparing `anwdlclient-1.1.1/anwdlclient/cli.py` & `anwdlclient-1.1.2/anwdlclient/cli.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/anwdlclient/config.py` & `anwdlclient-1.1.2/anwdlclient/config.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/anwdlclient/core/client.py` & `anwdlclient-1.1.2/anwdlclient/core/client.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/anwdlclient/core/crypto.py` & `anwdlclient-1.1.2/anwdlclient/core/crypto.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/anwdlclient/core/sanitize.py` & `anwdlclient-1.1.2/anwdlclient/core/sanitize.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/anwdlclient/core/util.py` & `anwdlclient-1.1.2/anwdlclient/core/util.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/anwdlclient/tools/accesstk.py` & `anwdlclient-1.1.2/anwdlclient/tools/accesstk.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/anwdlclient/tools/credentials.py` & `anwdlclient-1.1.2/anwdlclient/tools/credentials.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/anwdlclient.egg-info/SOURCES.txt` & `anwdlclient-1.1.2/anwdlclient.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CONTRIBUTING
 LICENSE
 MANIFEST.in
 README.md
 anwdlclient-uninstall
 anwdlclient-uninstall.bat
-pyproject.toml
 setup.py
 anwdlclient/__init__.py
 anwdlclient/cli.py
 anwdlclient/config.py
 anwdlclient.egg-info/PKG-INFO
 anwdlclient.egg-info/SOURCES.txt
 anwdlclient.egg-info/dependency_links.txt
```

### Comparing `anwdlclient-1.1.1/resources/config.yaml` & `anwdlclient-1.1.2/resources/config.yaml`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.1/setup.py` & `anwdlclient-1.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from subprocess import Popen, PIPE
 from setuptools import setup
 import getpass
 import shutil
 import os
 
-ACTUAL_VERSION = "1.1.1"
+ACTUAL_VERSION = "1.1.2"
 
 
 def executeCommand(command):
     Popen(command.split(" "), shell=False, stdout=PIPE, stderr=PIPE)
 
 
 anweddol_base_path = (
@@ -92,8 +92,11 @@
         "Topic :: System :: Emulators",
     ],
     license="GPL v3",
     url="https://github.com/the-anweddol-project/Anweddol-client",
     packages=["anwdlclient", "anwdlclient.core", "anwdlclient.tools"],
     install_requires=["cryptography", "cerberus", "pyyaml"],
     include_package_data=True,
+    entry_points={
+        "console_scripts": ["anwdlclient = anwdlclient.cli:MainAnweddolClientCLI"],
+    },
 )
```

