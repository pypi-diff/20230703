# Comparing `tmp/anwdlclient-1.1.0.tar.gz` & `tmp/anwdlclient-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anwdlclient-1.1.0.tar", last modified: Mon Jul  3 14:29:53 2023, max compression
+gzip compressed data, was "anwdlclient-1.1.1.tar", last modified: Mon Jul  3 14:46:06 2023, max compression
```

## Comparing `anwdlclient-1.1.0.tar` & `anwdlclient-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:29:53.214838 anwdlclient-1.1.0/
--rw-r--r--   0 user      (1001) user      (1001)     1150 2023-05-17 20:18:52.000000 anwdlclient-1.1.0/CONTRIBUTING
--rwxrwxrwx   0 user      (1001) user      (1001)    35129 2022-12-14 12:17:41.000000 anwdlclient-1.1.0/LICENSE
--rw-r--r--   0 user      (1001) user      (1001)      204 2023-07-03 14:12:19.000000 anwdlclient-1.1.0/MANIFEST.in
--rw-r--r--   0 user      (1001) user      (1001)    43787 2023-07-03 14:29:53.214838 anwdlclient-1.1.0/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     2425 2023-07-03 12:46:10.000000 anwdlclient-1.1.0/README.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:29:53.211838 anwdlclient-1.1.0/anwdlclient/
--rw-r--r--   0 user      (1001) user      (1001)       27 2023-07-03 12:16:43.000000 anwdlclient-1.1.0/anwdlclient/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)    42965 2023-07-03 09:54:55.000000 anwdlclient-1.1.0/anwdlclient/cli.py
--rw-r--r--   0 user      (1001) user      (1001)     1216 2023-05-30 16:26:10.000000 anwdlclient-1.1.0/anwdlclient/config.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:29:53.213838 anwdlclient-1.1.0/anwdlclient/core/
--rw-r--r--   0 user      (1001) user      (1001)        0 2023-04-10 17:55:16.000000 anwdlclient-1.1.0/anwdlclient/core/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     7119 2023-06-04 18:55:02.000000 anwdlclient-1.1.0/anwdlclient/core/client.py
--rwxrwxrwx   0 user      (1001) user      (1001)     7935 2023-05-16 08:04:03.000000 anwdlclient-1.1.0/anwdlclient/core/crypto.py
--rwxrwxrwx   0 user      (1001) user      (1001)     5807 2023-05-16 20:10:18.000000 anwdlclient-1.1.0/anwdlclient/core/sanitize.py
--rw-r--r--   0 user      (1001) user      (1001)     1182 2023-06-02 14:13:15.000000 anwdlclient-1.1.0/anwdlclient/core/util.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:29:53.214838 anwdlclient-1.1.0/anwdlclient/tools/
--rw-r--r--   0 user      (1001) user      (1001)        0 2023-04-22 13:25:26.000000 anwdlclient-1.1.0/anwdlclient/tools/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     2966 2023-06-11 11:17:13.000000 anwdlclient-1.1.0/anwdlclient/tools/accesstk.py
--rw-r--r--   0 user      (1001) user      (1001)     7096 2023-06-11 17:18:30.000000 anwdlclient-1.1.0/anwdlclient/tools/credentials.py
--rwxr-xr-x   0 user      (1001) user      (1001)      217 2023-07-03 12:51:38.000000 anwdlclient-1.1.0/anwdlclient-uninstall
--rw-r--r--   0 user      (1001) user      (1001)      232 2023-06-26 21:22:50.000000 anwdlclient-1.1.0/anwdlclient-uninstall.bat
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:29:53.212838 anwdlclient-1.1.0/anwdlclient.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)    43787 2023-07-03 14:29:53.000000 anwdlclient-1.1.0/anwdlclient.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)      643 2023-07-03 14:29:53.000000 anwdlclient-1.1.0/anwdlclient.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) user      (1001)        1 2023-07-03 14:29:53.000000 anwdlclient-1.1.0/anwdlclient.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) user      (1001)       70 2023-07-03 14:29:53.000000 anwdlclient-1.1.0/anwdlclient.egg-info/entry_points.txt
--rw-r--r--   0 user      (1001) user      (1001)       29 2023-07-03 14:29:53.000000 anwdlclient-1.1.0/anwdlclient.egg-info/requires.txt
--rw-r--r--   0 user      (1001) user      (1001)       12 2023-07-03 14:29:53.000000 anwdlclient-1.1.0/anwdlclient.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) user      (1001)     1033 2023-07-03 12:16:16.000000 anwdlclient-1.1.0/pyproject.toml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:29:53.214838 anwdlclient-1.1.0/resources/
--rw-r--r--   0 user      (1001) user      (1001)      668 2023-05-30 08:48:18.000000 anwdlclient-1.1.0/resources/config.yaml
--rw-r--r--   0 user      (1001) user      (1001)       38 2023-07-03 14:29:53.215838 anwdlclient-1.1.0/setup.cfg
--rw-r--r--   0 user      (1001) user      (1001)     3063 2023-07-03 14:04:02.000000 anwdlclient-1.1.0/setup.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.619700 anwdlclient-1.1.1/
+-rw-r--r--   0 user      (1001) user      (1001)     1150 2023-05-17 20:18:52.000000 anwdlclient-1.1.1/CONTRIBUTING
+-rwxrwxrwx   0 user      (1001) user      (1001)    35129 2022-12-14 12:17:41.000000 anwdlclient-1.1.1/LICENSE
+-rw-r--r--   0 user      (1001) user      (1001)      204 2023-07-03 14:12:19.000000 anwdlclient-1.1.1/MANIFEST.in
+-rw-r--r--   0 user      (1001) user      (1001)    43945 2023-07-03 14:46:06.619700 anwdlclient-1.1.1/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     2584 2023-07-03 14:32:39.000000 anwdlclient-1.1.1/README.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.616700 anwdlclient-1.1.1/anwdlclient/
+-rw-r--r--   0 user      (1001) user      (1001)       27 2023-07-03 14:45:25.000000 anwdlclient-1.1.1/anwdlclient/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)    42965 2023-07-03 09:54:55.000000 anwdlclient-1.1.1/anwdlclient/cli.py
+-rw-r--r--   0 user      (1001) user      (1001)     1216 2023-05-30 16:26:10.000000 anwdlclient-1.1.1/anwdlclient/config.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.618699 anwdlclient-1.1.1/anwdlclient/core/
+-rw-r--r--   0 user      (1001) user      (1001)        0 2023-04-10 17:55:16.000000 anwdlclient-1.1.1/anwdlclient/core/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     7119 2023-06-04 18:55:02.000000 anwdlclient-1.1.1/anwdlclient/core/client.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     7935 2023-05-16 08:04:03.000000 anwdlclient-1.1.1/anwdlclient/core/crypto.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     5807 2023-05-16 20:10:18.000000 anwdlclient-1.1.1/anwdlclient/core/sanitize.py
+-rw-r--r--   0 user      (1001) user      (1001)     1182 2023-06-02 14:13:15.000000 anwdlclient-1.1.1/anwdlclient/core/util.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.618699 anwdlclient-1.1.1/anwdlclient/tools/
+-rw-r--r--   0 user      (1001) user      (1001)        0 2023-04-22 13:25:26.000000 anwdlclient-1.1.1/anwdlclient/tools/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     2966 2023-06-11 11:17:13.000000 anwdlclient-1.1.1/anwdlclient/tools/accesstk.py
+-rw-r--r--   0 user      (1001) user      (1001)     7096 2023-06-11 17:18:30.000000 anwdlclient-1.1.1/anwdlclient/tools/credentials.py
+-rwxr-xr-x   0 user      (1001) user      (1001)      217 2023-07-03 12:51:38.000000 anwdlclient-1.1.1/anwdlclient-uninstall
+-rw-r--r--   0 user      (1001) user      (1001)      232 2023-06-26 21:22:50.000000 anwdlclient-1.1.1/anwdlclient-uninstall.bat
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.617699 anwdlclient-1.1.1/anwdlclient.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)    43945 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)      643 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) user      (1001)        1 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) user      (1001)       70 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1001) user      (1001)       29 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) user      (1001)       12 2023-07-03 14:46:06.000000 anwdlclient-1.1.1/anwdlclient.egg-info/top_level.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1033 2023-07-03 14:45:17.000000 anwdlclient-1.1.1/pyproject.toml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-07-03 14:46:06.619700 anwdlclient-1.1.1/resources/
+-rw-r--r--   0 user      (1001) user      (1001)      668 2023-05-30 08:48:18.000000 anwdlclient-1.1.1/resources/config.yaml
+-rw-r--r--   0 user      (1001) user      (1001)       38 2023-07-03 14:46:06.619700 anwdlclient-1.1.1/setup.cfg
+-rw-r--r--   0 user      (1001) user      (1001)     3079 2023-07-03 14:45:05.000000 anwdlclient-1.1.1/setup.py
```

### Comparing `anwdlclient-1.1.0/CONTRIBUTING` & `anwdlclient-1.1.1/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/LICENSE` & `anwdlclient-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/PKG-INFO` & `anwdlclient-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anwdlclient
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Anweddol client implementation
 Home-page: https://github.com/the-anweddol-project/Anweddol-client
 Author: The Anweddol project
 Author-email: The Anweddol project <the-anweddol-project@proton.me>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -714,28 +714,40 @@
 - The Anweddol client core features source code ;
 - The Anweddol client CLI implementation source code ;
 
 To get the server source code, see the [Anweddol server repository](https://github.com/the-anweddol-project/Anweddol-server).
 
 ## Installation
 
+### Pip installation
+
+Install it with pip (linux):
+```
+$ pip install anwdlclient
+```
+
+On windows : 
+```
+$ py -m pip install anwdlserver
+```
+
+### Source installation
+
 Clone the client source code repository : 
 ```
 $ git clone https://github.com/the-anweddol-project/Anweddol-client.git
-$ cd anweddol_client-v1.0.0
+$ cd Anweddol-client
 ```
 
 Install it with pip (linux):
-
 ```
 $ pip install .
 ```
 
-(Windows) : 
-
+On windows : 
 ```
 $ py -m pip install . 
 ```
 
 ## Configuration
 
 The Anweddol client implementation does not require specific setup to run.
```

### Comparing `anwdlclient-1.1.0/README.md` & `anwdlclient-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,28 +21,40 @@
 - The Anweddol client core features source code ;
 - The Anweddol client CLI implementation source code ;
 
 To get the server source code, see the [Anweddol server repository](https://github.com/the-anweddol-project/Anweddol-server).
 
 ## Installation
 
+### Pip installation
+
+Install it with pip (linux):
+```
+$ pip install anwdlclient
+```
+
+On windows : 
+```
+$ py -m pip install anwdlserver
+```
+
+### Source installation
+
 Clone the client source code repository : 
 ```
 $ git clone https://github.com/the-anweddol-project/Anweddol-client.git
-$ cd anweddol_client-v1.0.0
+$ cd Anweddol-client
 ```
 
 Install it with pip (linux):
-
 ```
 $ pip install .
 ```
 
-(Windows) : 
-
+On windows : 
 ```
 $ py -m pip install . 
 ```
 
 ## Configuration
 
 The Anweddol client implementation does not require specific setup to run.
@@ -72,8 +84,8 @@
 
 This is free software: you are free to change and redistribute it. There is NO WARRANTY, to the extent permitted by law.
 
 ## Developper / Maintainers list
 
 - Darnethal0z ([GitHub profile](https://github.com/Darnethal0z))
 
-*Copyright 2023 The Anweddol project*
+*Copyright 2023 The Anweddol project*
```

### Comparing `anwdlclient-1.1.0/anwdlclient/cli.py` & `anwdlclient-1.1.1/anwdlclient/cli.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/anwdlclient/config.py` & `anwdlclient-1.1.1/anwdlclient/config.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/anwdlclient/core/client.py` & `anwdlclient-1.1.1/anwdlclient/core/client.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/anwdlclient/core/crypto.py` & `anwdlclient-1.1.1/anwdlclient/core/crypto.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/anwdlclient/core/sanitize.py` & `anwdlclient-1.1.1/anwdlclient/core/sanitize.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/anwdlclient/core/util.py` & `anwdlclient-1.1.1/anwdlclient/core/util.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/anwdlclient/tools/accesstk.py` & `anwdlclient-1.1.1/anwdlclient/tools/accesstk.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/anwdlclient/tools/credentials.py` & `anwdlclient-1.1.1/anwdlclient/tools/credentials.py`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/anwdlclient.egg-info/PKG-INFO` & `anwdlclient-1.1.1/anwdlclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anwdlclient
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Anweddol client implementation
 Home-page: https://github.com/the-anweddol-project/Anweddol-client
 Author: The Anweddol project
 Author-email: The Anweddol project <the-anweddol-project@proton.me>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -714,28 +714,40 @@
 - The Anweddol client core features source code ;
 - The Anweddol client CLI implementation source code ;
 
 To get the server source code, see the [Anweddol server repository](https://github.com/the-anweddol-project/Anweddol-server).
 
 ## Installation
 
+### Pip installation
+
+Install it with pip (linux):
+```
+$ pip install anwdlclient
+```
+
+On windows : 
+```
+$ py -m pip install anwdlserver
+```
+
+### Source installation
+
 Clone the client source code repository : 
 ```
 $ git clone https://github.com/the-anweddol-project/Anweddol-client.git
-$ cd anweddol_client-v1.0.0
+$ cd Anweddol-client
 ```
 
 Install it with pip (linux):
-
 ```
 $ pip install .
 ```
 
-(Windows) : 
-
+On windows : 
 ```
 $ py -m pip install . 
 ```
 
 ## Configuration
 
 The Anweddol client implementation does not require specific setup to run.
```

### Comparing `anwdlclient-1.1.0/anwdlclient.egg-info/SOURCES.txt` & `anwdlclient-1.1.1/anwdlclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/pyproject.toml` & `anwdlclient-1.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tools.setuptools]
 packages = ["anwdlclient", "anwdlclient.core", "anwdlclient.tools"]
 
 [project]
 name = "anwdlclient"
-version = "1.1.0"
+version = "1.1.1"
 description = "The Anweddol client implementation"
 authors = [
   { name="The Anweddol project", email="the-anweddol-project@proton.me" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `anwdlclient-1.1.0/resources/config.yaml` & `anwdlclient-1.1.1/resources/config.yaml`

 * *Files identical despite different names*

### Comparing `anwdlclient-1.1.0/setup.py` & `anwdlclient-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from subprocess import Popen, PIPE
 from setuptools import setup
 import getpass
 import shutil
 import os
 
-ACTUAL_VERSION = "1.1.0"
+ACTUAL_VERSION = "1.1.1"
 
 
 def executeCommand(command):
     Popen(command.split(" "), shell=False, stdout=PIPE, stderr=PIPE)
 
 
 anweddol_base_path = (
@@ -67,15 +67,17 @@
     )
 
 else:
     shutil.copyfile(
         os.path.dirname(os.path.realpath(__file__)) + "/anwdlclient-uninstall",
         f"/home/{getpass.getuser()}/.local/bin/anwdlclient-uninstall",
     )
-    executeCommand(f"chmod +x /home/{getpass.getuser()}/.local/bin/anwdlclient-uninstall")
+    executeCommand(
+        f"chmod +x /home/{getpass.getuser()}/.local/bin/anwdlclient-uninstall"
+    )
 
 print("[SETUP] Installing Anweddol client ...")
 setup(
     name="anwdlclient",
     version=ACTUAL_VERSION,
     description="The Anweddol client implementation",
     author="The Anweddol project",
@@ -89,9 +91,9 @@
         "Topic :: Internet",
         "Topic :: System :: Emulators",
     ],
     license="GPL v3",
     url="https://github.com/the-anweddol-project/Anweddol-client",
     packages=["anwdlclient", "anwdlclient.core", "anwdlclient.tools"],
     install_requires=["cryptography", "cerberus", "pyyaml"],
-    include_package_data=True
-)
+    include_package_data=True,
+)
```

