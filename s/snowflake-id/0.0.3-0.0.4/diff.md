# Comparing `tmp/snowflake-id-0.0.3.tar.gz` & `tmp/snowflake-id-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-id-0.0.3.tar", last modified: Mon Jul  3 21:00:46 2023, max compression
+gzip compressed data, was "snowflake-id-0.0.4.tar", last modified: Mon Jul  3 21:00:43 2023, max compression
```

## Comparing `snowflake-id-0.0.3.tar` & `snowflake-id-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:00:46.371925 snowflake-id-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 21:00:35.000000 snowflake-id-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-03 21:00:46.371925 snowflake-id-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-03 21:00:35.000000 snowflake-id-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 21:00:46.371925 snowflake-id-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-03 21:00:35.000000 snowflake-id-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:00:46.367925 snowflake-id-0.0.3/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-03 21:00:35.000000 snowflake-id-0.0.3/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-03 21:00:35.000000 snowflake-id-0.0.3/snowflake/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:00:46.367925 snowflake-id-0.0.3/snowflake_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-03 21:00:46.000000 snowflake-id-0.0.3/snowflake_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 21:00:46.000000 snowflake-id-0.0.3/snowflake_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:00:46.000000 snowflake-id-0.0.3/snowflake_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 21:00:46.000000 snowflake-id-0.0.3/snowflake_id.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:00:43.680906 snowflake-id-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 21:00:32.000000 snowflake-id-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-03 21:00:43.680906 snowflake-id-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-03 21:00:32.000000 snowflake-id-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 21:00:43.680906 snowflake-id-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-03 21:00:32.000000 snowflake-id-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:00:43.680906 snowflake-id-0.0.4/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-03 21:00:32.000000 snowflake-id-0.0.4/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-03 21:00:32.000000 snowflake-id-0.0.4/snowflake/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:00:43.680906 snowflake-id-0.0.4/snowflake_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-03 21:00:43.000000 snowflake-id-0.0.4/snowflake_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 21:00:43.000000 snowflake-id-0.0.4/snowflake_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:00:43.000000 snowflake-id-0.0.4/snowflake_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 21:00:43.000000 snowflake-id-0.0.4/snowflake_id.egg-info/top_level.txt
```

### Comparing `snowflake-id-0.0.3/LICENSE` & `snowflake-id-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-id-0.0.3/PKG-INFO` & `snowflake-id-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-id
-Version: 0.0.3
+Version: 0.0.4
 Summary: The Snowflake generator done right.
 Home-page: https://github.com/vd2org/snowflake
 Author: Vd
 Author-email: vd@vd2.org
 License: MIT
 Description: # Snowflake
         
@@ -107,14 +107,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
 Classifier: Topic :: Internet
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `snowflake-id-0.0.3/README.md` & `snowflake-id-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-id-0.0.3/setup.py` & `snowflake-id-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from os.path import join, dirname
 
 import setuptools
 
 setuptools.setup(
     name='snowflake-id',
-    version='0.0.3',
+    version='0.0.4',
     author='Vd',
     author_email='vd@vd2.org',
     url='https://github.com/vd2org/snowflake',
     license='MIT',
     description='The Snowflake generator done right.',
     long_description=open(join(dirname(__file__), 'README.md')).read(),
     long_description_content_type='text/markdown',
@@ -26,14 +26,15 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Database',
         'Topic :: Internet',
         'Topic :: Utilities',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

### Comparing `snowflake-id-0.0.3/snowflake/snowflake.py` & `snowflake-id-0.0.4/snowflake/snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     def __int__(self) -> int:
         return self.value
 
 
 class SnowflakeGenerator:
     def __init__(self, instance: int, *, seq: int = 0, epoch: int = 0, timestamp: Optional[int] = None):
 
-        current = int(time() * 1000)
+        current = int(time() * 1000.)
 
         if current - epoch >= MAX_TS:
             raise OverflowError(f"The maximum current timestamp has been reached in selected epoch,"
                                 f"so Snowflake cannot generate more IDs!")
 
         timestamp = timestamp or current
 
@@ -108,15 +108,15 @@
     def epoch(self) -> int:
         return self._epo
 
     def __iter__(self):
         return self
 
     def __next__(self) -> Optional[int]:
-        current = int(time() * 1000) - self._epo
+        current = int(time() * 1000.) - self._epo
 
         if current >= MAX_TS:
             raise OverflowError(f"The maximum current timestamp has been reached in selected epoch,"
                                 f"so Snowflake cannot generate more IDs!")
 
         if self._ts == current:
             if self._seq == MAX_SEQ:
```

### Comparing `snowflake-id-0.0.3/snowflake_id.egg-info/PKG-INFO` & `snowflake-id-0.0.4/snowflake_id.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-id
-Version: 0.0.3
+Version: 0.0.4
 Summary: The Snowflake generator done right.
 Home-page: https://github.com/vd2org/snowflake
 Author: Vd
 Author-email: vd@vd2.org
 License: MIT
 Description: # Snowflake
         
@@ -107,14 +107,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
 Classifier: Topic :: Internet
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

