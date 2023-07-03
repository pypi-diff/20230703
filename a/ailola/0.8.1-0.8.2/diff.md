# Comparing `tmp/ailola-0.8.1.tar.gz` & `tmp/ailola-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailola-0.8.1.tar", last modified: Mon Jul  3 08:57:03 2023, max compression
+gzip compressed data, was "ailola-0.8.2.tar", last modified: Mon Jul  3 08:59:59 2023, max compression
```

## Comparing `ailola-0.8.1.tar` & `ailola-0.8.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:57:03.817803 ailola-0.8.1/
--rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 08:57:03.817952 ailola-0.8.1/PKG-INFO
--rw-r--r--   0 elhayefrat   (501) staff       (20)       16 2023-07-03 07:44:46.000000 ailola-0.8.1/README.md
-drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:57:03.759634 ailola-0.8.1/ailola/
-drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:57:03.816453 ailola-0.8.1/ailola/ailola.egg-info/
--rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 08:57:03.000000 ailola-0.8.1/ailola/ailola.egg-info/PKG-INFO
--rw-r--r--   0 elhayefrat   (501) staff       (20)      252 2023-07-03 08:57:03.000000 ailola-0.8.1/ailola/ailola.egg-info/SOURCES.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)        1 2023-07-03 08:57:03.000000 ailola-0.8.1/ailola/ailola.egg-info/dependency_links.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)       38 2023-07-03 08:57:03.000000 ailola-0.8.1/ailola/ailola.egg-info/entry_points.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)       22 2023-07-03 08:57:03.000000 ailola-0.8.1/ailola/ailola.egg-info/requires.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)        1 2023-07-03 08:57:03.000000 ailola-0.8.1/ailola/ailola.egg-info/top_level.txt
--rw-r--r--   0 elhayefrat   (501) staff       (20)      107 2023-07-03 08:57:03.818879 ailola-0.8.1/setup.cfg
--rw-r--r--   0 elhayefrat   (501) staff       (20)      774 2023-07-03 08:56:43.000000 ailola-0.8.1/setup.py
+drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:59:59.779691 ailola-0.8.2/
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 08:59:59.779775 ailola-0.8.2/PKG-INFO
+-rw-r--r--   0 elhayefrat   (501) staff       (20)       16 2023-07-03 07:44:46.000000 ailola-0.8.2/README.md
+drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:59:59.760949 ailola-0.8.2/ailola/
+-rw-r--r--   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:51:51.000000 ailola-0.8.2/ailola/__init__.py
+drwxr-xr-x   0 elhayefrat   (501) staff       (20)        0 2023-07-03 08:59:59.779061 ailola-0.8.2/ailola/ailola.egg-info/
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      197 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/PKG-INFO
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      288 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/SOURCES.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)        1 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/dependency_links.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)       38 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/entry_points.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)       22 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/requires.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)       16 2023-07-03 08:59:59.000000 ailola-0.8.2/ailola/ailola.egg-info/top_level.txt
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      236 2023-07-03 08:43:53.000000 ailola-0.8.2/ailola/ailola.py
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      107 2023-07-03 08:59:59.780246 ailola-0.8.2/setup.cfg
+-rw-r--r--   0 elhayefrat   (501) staff       (20)      812 2023-07-03 08:59:58.000000 ailola-0.8.2/setup.py
```

### Comparing `ailola-0.8.1/setup.py` & `ailola-0.8.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='ailola',
-    version='0.8.1',
+    version='0.8.2',
     license='MIT',
     author="Elhay Efrat",
     author_email='elhayefrat@gmail.com',
-    packages=find_packages('ailola'),
-    package_dir={'': 'ailola'},
+    # packages=find_packages('ailola'),
+    # package_dir={'': 'ailola'},
+    package_dir = {'': 'ailola'},
     url='https://github.com/lola-pola/ailola',
     keywords='lola cli terraform ai',
     install_requires=['click', 'requests' ,'openai'],
     entry_points={'console_scripts': ['ailola = ailola:cli']}
 
 )
```

