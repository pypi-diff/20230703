# Comparing `tmp/jsoner-lib-0.4.tar.gz` & `tmp/jsoner-lib-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsoner-lib-0.4.tar", last modified: Mon Jul  3 01:28:55 2023, max compression
+gzip compressed data, was "jsoner-lib-0.5.tar", last modified: Mon Jul  3 01:42:38 2023, max compression
```

## Comparing `jsoner-lib-0.4.tar` & `jsoner-lib-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 01:28:55.063619 jsoner-lib-0.4/
--rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-03 00:29:20.000000 jsoner-lib-0.4/LICENSE
--rw-r--r--   0 bigmag_    (502) staff       (20)     1916 2023-07-03 01:28:55.063110 jsoner-lib-0.4/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)     1673 2023-07-03 00:57:05.000000 jsoner-lib-0.4/README.md
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 01:28:55.058857 jsoner-lib-0.4/jsoner/
--rw-r--r--   0 bigmag_    (502) staff       (20)       49 2023-07-02 23:41:44.000000 jsoner-lib-0.4/jsoner/__init__.py
--rw-r--r--   0 bigmag_    (502) staff       (20)     2563 2023-07-02 23:46:21.000000 jsoner-lib-0.4/jsoner/main.py
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 01:28:55.062164 jsoner-lib-0.4/jsoner_lib.egg-info/
--rw-r--r--   0 bigmag_    (502) staff       (20)     1916 2023-07-03 01:28:54.000000 jsoner-lib-0.4/jsoner_lib.egg-info/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)      229 2023-07-03 01:28:54.000000 jsoner-lib-0.4/jsoner_lib.egg-info/SOURCES.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 01:28:54.000000 jsoner-lib-0.4/jsoner_lib.egg-info/dependency_links.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        9 2023-07-03 01:28:54.000000 jsoner-lib-0.4/jsoner_lib.egg-info/requires.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        7 2023-07-03 01:28:54.000000 jsoner-lib-0.4/jsoner_lib.egg-info/top_level.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-03 01:28:55.063742 jsoner-lib-0.4/setup.cfg
--rw-r--r--   0 bigmag_    (502) staff       (20)      552 2023-07-03 01:28:42.000000 jsoner-lib-0.4/setup.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 01:42:38.357461 jsoner-lib-0.5/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-03 00:29:20.000000 jsoner-lib-0.5/LICENSE
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1940 2023-07-03 01:42:38.357728 jsoner-lib-0.5/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1673 2023-07-03 00:57:05.000000 jsoner-lib-0.5/README.md
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 01:42:38.352257 jsoner-lib-0.5/jsoner/
+-rw-r--r--   0 bigmag_    (502) staff       (20)       49 2023-07-02 23:41:44.000000 jsoner-lib-0.5/jsoner/__init__.py
+-rw-r--r--   0 bigmag_    (502) staff       (20)     2563 2023-07-02 23:46:21.000000 jsoner-lib-0.5/jsoner/main.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-03 01:42:38.356742 jsoner-lib-0.5/jsoner_lib.egg-info/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1940 2023-07-03 01:42:38.000000 jsoner-lib-0.5/jsoner_lib.egg-info/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)      239 2023-07-03 01:42:38.000000 jsoner-lib-0.5/jsoner_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-03 01:42:38.000000 jsoner-lib-0.5/jsoner_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        9 2023-07-03 01:42:38.000000 jsoner-lib-0.5/jsoner_lib.egg-info/requires.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        7 2023-07-03 01:42:38.000000 jsoner-lib-0.5/jsoner_lib.egg-info/top_level.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-03 01:42:38.359083 jsoner-lib-0.5/setup.cfg
+-rw-r--r--   0 bigmag_    (502) staff       (20)      581 2023-07-03 01:41:43.000000 jsoner-lib-0.5/setup.py
```

### Comparing `jsoner-lib-0.4/LICENSE` & `jsoner-lib-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsoner-lib-0.4/PKG-INFO` & `jsoner-lib-0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jsoner-lib
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/kradt/jsoner
 Author: kradt
 Author-email: sidorenkoarem950@gmail.com
 License: MIT
 Keywords: jsoner
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jsoner
 
 Convenient and fast adding objects to json file
```

### Comparing `jsoner-lib-0.4/README.md` & `jsoner-lib-0.5/README.md`

 * *Files identical despite different names*

### Comparing `jsoner-lib-0.4/jsoner/main.py` & `jsoner-lib-0.5/jsoner/main.py`

 * *Files identical despite different names*

### Comparing `jsoner-lib-0.4/jsoner_lib.egg-info/PKG-INFO` & `jsoner-lib-0.5/jsoner_lib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jsoner-lib
-Version: 0.4
+Version: 0.5
 Home-page: https://github.com/kradt/jsoner
 Author: kradt
 Author-email: sidorenkoarem950@gmail.com
 License: MIT
 Keywords: jsoner
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jsoner
 
 Convenient and fast adding objects to json file
```

### Comparing `jsoner-lib-0.4/setup.py` & `jsoner-lib-0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='jsoner-lib',
-    version='0.4',
+    version='0.5',
     license='MIT',
     author="kradt",
     author_email='sidorenkoarem950@gmail.com',
     packages=find_packages(),
     url='https://github.com/kradt/jsoner',
     keywords='jsoner',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
           'pydantic',
       ],
+    python_requires='>=3.11'
 
 )
```

