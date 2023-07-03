# Comparing `tmp/workstation_shell-0.0.1.tar.gz` & `tmp/workstation_shell-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workstation_shell-0.0.1.tar", last modified: Mon Jul  3 08:52:31 2023, max compression
+gzip compressed data, was "workstation_shell-0.0.2.tar", last modified: Mon Jul  3 09:37:34 2023, max compression
```

## Comparing `workstation_shell-0.0.1.tar` & `workstation_shell-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2023-07-03 08:52:31.620935 workstation_shell-0.0.1/
--rw-rw-r--   0 hx        (1000) hx        (1000)      303 2023-07-03 08:52:31.620935 workstation_shell-0.0.1/PKG-INFO
--rw-rw-r--   0 hx        (1000) hx        (1000)       20 2023-07-03 08:51:45.000000 workstation_shell-0.0.1/README.md
--rw-rw-r--   0 hx        (1000) hx        (1000)       38 2023-07-03 08:52:31.620935 workstation_shell-0.0.1/setup.cfg
--rwxrwxr-x   0 hx        (1000) hx        (1000)      645 2023-07-03 08:52:08.000000 workstation_shell-0.0.1/setup.py
-drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2023-07-03 08:52:31.620935 workstation_shell-0.0.1/workstation_shell.egg-info/
--rw-rw-r--   0 hx        (1000) hx        (1000)      303 2023-07-03 08:52:31.000000 workstation_shell-0.0.1/workstation_shell.egg-info/PKG-INFO
--rw-rw-r--   0 hx        (1000) hx        (1000)      266 2023-07-03 08:52:31.000000 workstation_shell-0.0.1/workstation_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 hx        (1000) hx        (1000)        1 2023-07-03 08:52:31.000000 workstation_shell-0.0.1/workstation_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 hx        (1000) hx        (1000)       61 2023-07-03 08:52:31.000000 workstation_shell-0.0.1/workstation_shell.egg-info/entry_points.txt
--rw-rw-r--   0 hx        (1000) hx        (1000)       14 2023-07-03 08:52:31.000000 workstation_shell-0.0.1/workstation_shell.egg-info/requires.txt
--rw-rw-r--   0 hx        (1000) hx        (1000)        1 2023-07-03 08:52:31.000000 workstation_shell-0.0.1/workstation_shell.egg-info/top_level.txt
+drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2023-07-03 09:37:34.249537 workstation_shell-0.0.2/
+-rw-rw-r--   0 hx        (1000) hx        (1000)      303 2023-07-03 09:37:34.249537 workstation_shell-0.0.2/PKG-INFO
+-rw-rw-r--   0 hx        (1000) hx        (1000)       20 2023-07-03 09:33:26.000000 workstation_shell-0.0.2/README.md
+-rw-rw-r--   0 hx        (1000) hx        (1000)       38 2023-07-03 09:37:34.249537 workstation_shell-0.0.2/setup.cfg
+-rwxrwxr-x   0 hx        (1000) hx        (1000)      659 2023-07-03 09:36:10.000000 workstation_shell-0.0.2/setup.py
+drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2023-07-03 09:37:34.249537 workstation_shell-0.0.2/workstation_shell/
+-rw-rw-r--   0 hx        (1000) hx        (1000)        0 2023-07-03 09:33:40.000000 workstation_shell-0.0.2/workstation_shell/__init__.py
+-rwxrwxr-x   0 hx        (1000) hx        (1000)     3250 2023-07-03 09:33:40.000000 workstation_shell-0.0.2/workstation_shell/workstation_shell.py
+drwxrwxr-x   0 hx        (1000) hx        (1000)        0 2023-07-03 09:37:34.249537 workstation_shell-0.0.2/workstation_shell.egg-info/
+-rw-rw-r--   0 hx        (1000) hx        (1000)      303 2023-07-03 09:37:34.000000 workstation_shell-0.0.2/workstation_shell.egg-info/PKG-INFO
+-rw-rw-r--   0 hx        (1000) hx        (1000)      335 2023-07-03 09:37:34.000000 workstation_shell-0.0.2/workstation_shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 hx        (1000) hx        (1000)        1 2023-07-03 09:37:34.000000 workstation_shell-0.0.2/workstation_shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 hx        (1000) hx        (1000)       79 2023-07-03 09:37:34.000000 workstation_shell-0.0.2/workstation_shell.egg-info/entry_points.txt
+-rw-rw-r--   0 hx        (1000) hx        (1000)       14 2023-07-03 09:37:34.000000 workstation_shell-0.0.2/workstation_shell.egg-info/requires.txt
+-rw-rw-r--   0 hx        (1000) hx        (1000)       18 2023-07-03 09:37:34.000000 workstation_shell-0.0.2/workstation_shell.egg-info/top_level.txt
```

### Comparing `workstation_shell-0.0.1/setup.py` & `workstation_shell-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='workstation_shell',
-    version='0.0.1',
+    version='0.0.2',
     install_requires=[
         'msgpack',
-        'pyzmq',
+        'pyzmq'
     ],
     packages=find_packages(),
     author='liutelin',
     author_email='liutelin@cvte.com',
     description='workstation shell command line tools.',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     entry_points={  # Optional
         "console_scripts": [
-            "workstation_shell=workstation_shell:main"
-        ],
+            "workstation_shell=workstation_shell.workstation_shell:main"
+        ]
     }
-
 )
```

