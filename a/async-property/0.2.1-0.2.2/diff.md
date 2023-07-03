# Comparing `tmp/async_property-0.2.1.tar.gz` & `tmp/async_property-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/async_property-0.2.1.tar", last modified: Sun Apr 14 03:34:21 2019, max compression
+gzip compressed data, was "async_property-0.2.2.tar", last modified: Mon Jul  3 17:21:53 2023, max compression
```

## Comparing `async_property-0.2.1.tar` & `async_property-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-14 03:34:21.000000 async_property-0.2.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3605 2019-04-14 03:33:24.000000 async_property-0.2.1/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      524 2019-04-14 03:33:24.000000 async_property-0.2.1/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2019-04-14 03:33:24.000000 async_property-0.2.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      242 2019-04-14 03:33:24.000000 async_property-0.2.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     6474 2019-04-14 03:34:21.000000 async_property-0.2.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3787 2019-04-14 03:33:24.000000 async_property-0.2.1/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-14 03:34:21.000000 async_property-0.2.1/async_property/
--rw-rw-r--   0 travis    (2000) travis    (2000)      323 2019-04-14 03:33:24.000000 async_property-0.2.1/async_property/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1279 2019-04-14 03:33:24.000000 async_property-0.2.1/async_property/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3948 2019-04-14 03:33:24.000000 async_property-0.2.1/async_property/cached.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2019-04-14 03:33:24.000000 async_property-0.2.1/async_property/loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13028 2019-04-14 03:33:24.000000 async_property-0.2.1/async_property/proxy.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-14 03:34:21.000000 async_property-0.2.1/async_property.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6474 2019-04-14 03:34:21.000000 async_property-0.2.1/async_property.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      681 2019-04-14 03:34:21.000000 async_property-0.2.1/async_property.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-04-14 03:34:21.000000 async_property-0.2.1/async_property.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-04-14 03:34:21.000000 async_property-0.2.1/async_property.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2019-04-14 03:34:21.000000 async_property-0.2.1/async_property.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-14 03:34:21.000000 async_property-0.2.1/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2019-04-14 03:33:24.000000 async_property-0.2.1/docs/Makefile
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4903 2019-04-14 03:33:24.000000 async_property-0.2.1/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-04-14 03:33:24.000000 async_property-0.2.1/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-04-14 03:33:24.000000 async_property-0.2.1/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      284 2019-04-14 03:33:24.000000 async_property-0.2.1/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1273 2019-04-14 03:33:24.000000 async_property-0.2.1/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      776 2019-04-14 03:33:24.000000 async_property-0.2.1/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2019-04-14 03:33:24.000000 async_property-0.2.1/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      456 2019-04-14 03:34:21.000000 async_property-0.2.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1275 2019-04-14 03:33:24.000000 async_property-0.2.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-14 03:34:21.000000 async_property-0.2.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-04-14 03:33:24.000000 async_property-0.2.1/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3075 2019-04-14 03:33:24.000000 async_property-0.2.1/tests/test_async_cached_property.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1164 2019-04-14 03:33:24.000000 async_property-0.2.1/tests/test_async_property.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2019-04-14 03:33:24.000000 async_property-0.2.1/tests/test_asyncio_lock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      958 2019-04-14 03:33:24.000000 async_property-0.2.1/tests/test_inheritance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1216 2019-04-14 03:33:24.000000 async_property-0.2.1/tests/test_loader.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-03 17:21:53.560038 async_property-0.2.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3605 2023-07-03 17:20:59.000000 async_property-0.2.2/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      611 2023-07-03 17:20:59.000000 async_property-0.2.2/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1072 2023-07-03 17:20:59.000000 async_property-0.2.2/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      242 2023-07-03 17:20:59.000000 async_property-0.2.2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5289 2023-07-03 17:21:53.560038 async_property-0.2.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3832 2023-07-03 17:20:59.000000 async_property-0.2.2/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-03 17:21:53.556037 async_property-0.2.2/async_property/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      323 2023-07-03 17:20:59.000000 async_property-0.2.2/async_property/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1279 2023-07-03 17:20:59.000000 async_property-0.2.2/async_property/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3948 2023-07-03 17:20:59.000000 async_property-0.2.2/async_property/cached.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1398 2023-07-03 17:20:59.000000 async_property-0.2.2/async_property/loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13028 2023-07-03 17:20:59.000000 async_property-0.2.2/async_property/proxy.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-03 17:21:53.560038 async_property-0.2.2/async_property.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5289 2023-07-03 17:21:53.000000 async_property-0.2.2/async_property.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      681 2023-07-03 17:21:53.000000 async_property-0.2.2/async_property.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-03 17:21:53.000000 async_property-0.2.2/async_property.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-03 17:21:53.000000 async_property-0.2.2/async_property.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       15 2023-07-03 17:21:53.000000 async_property-0.2.2/async_property.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-03 17:21:53.560038 async_property-0.2.2/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      615 2023-07-03 17:20:59.000000 async_property-0.2.2/docs/Makefile
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4903 2023-07-03 17:20:59.000000 async_property-0.2.2/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2023-07-03 17:20:59.000000 async_property-0.2.2/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2023-07-03 17:20:59.000000 async_property-0.2.2/docs/history.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      284 2023-07-03 17:20:59.000000 async_property-0.2.2/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1273 2023-07-03 17:20:59.000000 async_property-0.2.2/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      776 2023-07-03 17:20:59.000000 async_property-0.2.2/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)       27 2023-07-03 17:20:59.000000 async_property-0.2.2/docs/readme.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      446 2023-07-03 17:21:53.560038 async_property-0.2.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1490 2023-07-03 17:20:59.000000 async_property-0.2.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-03 17:21:53.560038 async_property-0.2.2/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-03 17:20:59.000000 async_property-0.2.2/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3075 2023-07-03 17:20:59.000000 async_property-0.2.2/tests/test_async_cached_property.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1164 2023-07-03 17:20:59.000000 async_property-0.2.2/tests/test_async_property.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2023-07-03 17:20:59.000000 async_property-0.2.2/tests/test_asyncio_lock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      958 2023-07-03 17:20:59.000000 async_property-0.2.2/tests/test_inheritance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1216 2023-07-03 17:20:59.000000 async_property-0.2.2/tests/test_loader.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `async_property-0.2.1/CONTRIBUTING.rst` & `async_property-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/LICENSE` & `async_property-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/README.rst` & `async_property-0.2.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 async_property
 ==============
 
 
 .. image:: https://img.shields.io/pypi/v/async_property.svg
     :target: https://pypi.org/project/async-property/
 
-.. image:: https://img.shields.io/travis/ryananguiano/async_property.svg
-    :target: https://travis-ci.org/ryananguiano/async_property
+.. image:: https://app.travis-ci.com/ryananguiano/async_property.svg?branch=master
+    :target: https://app.travis-ci.com/github/ryananguiano/async_property
 
 .. image:: https://readthedocs.org/projects/async-property/badge/?version=latest
     :target: https://async-property.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. image:: https://pyup.io/repos/github/ryananguiano/async_property/shield.svg
     :target: https://pyup.io/repos/github/ryananguiano/async_property/
     :alt: Updates
 
 
 Python decorator for async properties.
 
+* Python: 3.7+
 * Free software: MIT license
 * Documentation: https://async-property.readthedocs.io
 * Package: https://pypi.org/project/async-property
 * Source code: https://github.com/ryananguiano/async_property
 
 Install
 -------
@@ -113,29 +114,31 @@
 
         @async_cached_property
         async def db_lookup(self):
             return 'success'
 
         @async_cached_property
         async def api_call(self):
+            print('calling api')
             return 'works every time'
 
     >>> instance = await Foo()
     load called
+    calling api
     >>> instance.db_lookup
     'success'
     >>> instance.api_call
     'works every time'
 
 Features
 --------
 
 * Both regular and cached property.
-* ``@async_cached_property`` can be accessed multiple times without repeating function call.
-* ``@async_cached_property`` uses asyncio.Lock to ensure function is called only once per instance.
+* Cached properties can be accessed multiple times without repeating function call.
+* Uses asyncio.Lock to ensure cached functions are called only once.
 * Full test coverage with py.test
 
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
```

### Comparing `async_property-0.2.1/async_property/base.py` & `async_property-0.2.2/async_property/base.py`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/async_property/cached.py` & `async_property-0.2.2/async_property/cached.py`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/async_property/loader.py` & `async_property-0.2.2/async_property/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,12 +37,12 @@
         and then calls async property loaders
         """
         if hasattr(self, 'load') and is_coroutine(self.load):
             await self.load()
         loaders = get_loaders(self)
         if loaders:
             await asyncio.wait([
-                get_loader(self)()
+                asyncio.create_task(get_loader(self)())
                 for field, get_loader
                 in loaders
             ])
         return self
```

### Comparing `async_property-0.2.1/async_property/proxy.py` & `async_property-0.2.2/async_property/proxy.py`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/async_property.egg-info/SOURCES.txt` & `async_property-0.2.2/async_property.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/docs/Makefile` & `async_property-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/docs/conf.py` & `async_property-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/docs/installation.rst` & `async_property-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/docs/make.bat` & `async_property-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/setup.py` & `async_property-0.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,30 +15,35 @@
 
 test_requirements = ['pytest']
 
 setup(
     author="Ryan Anguiano",
     author_email='ryan.anguiano@gmail.com',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Software Development',
+        'Topic :: Utilities',
     ],
     description="Python decorator for async properties.",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='async_property',
     name='async_property',
     packages=find_packages(include=['async_property']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ryananguiano/async_property',
-    version='0.2.1',
+    version='0.2.2',
     zip_safe=False,
 )
```

### Comparing `async_property-0.2.1/tests/test_async_cached_property.py` & `async_property-0.2.2/tests/test_async_cached_property.py`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/tests/test_async_property.py` & `async_property-0.2.2/tests/test_async_property.py`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/tests/test_asyncio_lock.py` & `async_property-0.2.2/tests/test_asyncio_lock.py`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/tests/test_inheritance.py` & `async_property-0.2.2/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `async_property-0.2.1/tests/test_loader.py` & `async_property-0.2.2/tests/test_loader.py`

 * *Files identical despite different names*

