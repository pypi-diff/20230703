# Comparing `tmp/px-django-lingua-0.1.7.tar.gz` & `tmp/px-django-lingua-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "px-django-lingua-0.1.7.tar", last modified: Fri Apr 28 10:12:07 2023, max compression
+gzip compressed data, was "px-django-lingua-0.1.8.tar", last modified: Mon Jul  3 13:49:03 2023, max compression
```

## Comparing `px-django-lingua-0.1.7.tar` & `px-django-lingua-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-28 10:12:07.684660 px-django-lingua-0.1.7/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1079 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/LICENSE
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9676 2023-04-28 10:12:07.684660 px-django-lingua-0.1.7/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9060 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/README.md
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-28 10:12:07.684660 px-django-lingua-0.1.7/px_django_lingua.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     9676 2023-04-28 10:12:07.000000 px-django-lingua-0.1.7/px_django_lingua.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      480 2023-04-28 10:12:07.000000 px-django-lingua-0.1.7/px_django_lingua.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-04-28 10:12:07.000000 px-django-lingua-0.1.7/px_django_lingua.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      149 2023-04-28 10:12:07.000000 px-django-lingua-0.1.7/px_django_lingua.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       11 2023-04-28 10:12:07.000000 px-django-lingua-0.1.7/px_django_lingua.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-04-28 10:12:07.684660 px-django-lingua-0.1.7/pxd_lingua/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      139 2023-04-28 10:12:01.000000 px-django-lingua-0.1.7/pxd_lingua/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      140 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/admin.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      229 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      893 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1550 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/db.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      172 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/exceptions.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1454 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/loader.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     8069 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/magic.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5010 2023-04-28 10:11:50.000000 px-django-lingua-0.1.7/pxd_lingua/models.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1733 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/query.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      139 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/types.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1737 2023-04-28 09:37:51.000000 px-django-lingua-0.1.7/pxd_lingua/utils.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       79 2023-04-28 10:12:07.684660 px-django-lingua-0.1.7/setup.cfg
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1494 2023-04-28 09:48:29.000000 px-django-lingua-0.1.7/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-07-03 13:49:03.972131 px-django-lingua-0.1.8/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1079 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/LICENSE
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9676 2023-07-03 13:49:03.972131 px-django-lingua-0.1.8/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9060 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/README.md
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-07-03 13:49:03.968131 px-django-lingua-0.1.8/px_django_lingua.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     9676 2023-07-03 13:49:03.000000 px-django-lingua-0.1.8/px_django_lingua.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      480 2023-07-03 13:49:03.000000 px-django-lingua-0.1.8/px_django_lingua.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-07-03 13:49:03.000000 px-django-lingua-0.1.8/px_django_lingua.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      149 2023-07-03 13:49:03.000000 px-django-lingua-0.1.8/px_django_lingua.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       11 2023-07-03 13:49:03.000000 px-django-lingua-0.1.8/px_django_lingua.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-07-03 13:49:03.972131 px-django-lingua-0.1.8/pxd_lingua/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      139 2023-07-03 13:48:51.000000 px-django-lingua-0.1.8/pxd_lingua/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      140 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/admin.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      229 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      893 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1550 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/db.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      172 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/exceptions.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1454 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/loader.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     8069 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/magic.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5010 2023-04-28 10:11:50.000000 px-django-lingua-0.1.8/pxd_lingua/models.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1733 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/query.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      139 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/types.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1737 2023-04-28 09:37:51.000000 px-django-lingua-0.1.8/pxd_lingua/utils.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       79 2023-07-03 13:49:03.972131 px-django-lingua-0.1.8/setup.cfg
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1494 2023-07-03 13:47:14.000000 px-django-lingua-0.1.8/setup.py
```

### Comparing `px-django-lingua-0.1.7/LICENSE` & `px-django-lingua-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.7/PKG-INFO` & `px-django-lingua-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: px-django-lingua
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple translations implementation for django models.
 Home-page: UNKNOWN
 Author: Alex Tkachenko
 Author-email: preusx.dev@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `px-django-lingua-0.1.7/README.md` & `px-django-lingua-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.7/px_django_lingua.egg-info/PKG-INFO` & `px-django-lingua-0.1.8/px_django_lingua.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: px-django-lingua
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple translations implementation for django models.
 Home-page: UNKNOWN
 Author: Alex Tkachenko
 Author-email: preusx.dev@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `px-django-lingua-0.1.7/pxd_lingua/conf.py` & `px-django-lingua-0.1.8/pxd_lingua/conf.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.7/pxd_lingua/db.py` & `px-django-lingua-0.1.8/pxd_lingua/db.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.7/pxd_lingua/loader.py` & `px-django-lingua-0.1.8/pxd_lingua/loader.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.7/pxd_lingua/magic.py` & `px-django-lingua-0.1.8/pxd_lingua/magic.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.7/pxd_lingua/models.py` & `px-django-lingua-0.1.8/pxd_lingua/models.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.7/pxd_lingua/query.py` & `px-django-lingua-0.1.8/pxd_lingua/query.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.7/pxd_lingua/utils.py` & `px-django-lingua-0.1.8/pxd_lingua/utils.py`

 * *Files identical despite different names*

### Comparing `px-django-lingua-0.1.7/setup.py` & `px-django-lingua-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     version=version,
     author='Alex Tkachenko',
     author_email='preusx.dev@gmail.com',
     license='MIT License',
     description='Simple translations implementation for django models.',
     install_requires=[
         'px-settings>=0.1.2,<0.2.0',
-        'django>=2.2,<4',
+        'django>=2.2,<5',
     ],
     extras_require={
         'dev': [
             'pytest>=6.0,<7.0',
             'pytest-watch>=4.2,<5.0',
             'pytest-django>=4.3,<5.0',
             'django-environ',
```

