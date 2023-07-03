# Comparing `tmp/django-timestampable-1.1.1.tar.gz` & `tmp/django-timestampable-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-timestampable-1.1.1.tar", last modified: Sat Mar  4 13:40:53 2023, max compression
+gzip compressed data, was "django-timestampable-1.1.2.tar", last modified: Mon Jul  3 09:20:32 2023, max compression
```

## Comparing `django-timestampable-1.1.1.tar` & `django-timestampable-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-03-04 13:40:53.758679 django-timestampable-1.1.1/
--rw-r--r--   0 dmp593     (501) staff       (20)     1063 2022-11-12 11:31:09.000000 django-timestampable-1.1.1/LICENSE
--rw-r--r--   0 dmp593     (501) staff       (20)       58 2022-11-12 11:31:09.000000 django-timestampable-1.1.1/MANIFEST.in
--rw-r--r--   0 dmp593     (501) staff       (20)    10034 2023-03-04 13:40:53.758762 django-timestampable-1.1.1/PKG-INFO
--rw-r--r--   0 dmp593     (501) staff       (20)     8718 2023-03-04 13:34:41.000000 django-timestampable-1.1.1/README.md
-drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-03-04 13:40:53.757025 django-timestampable-1.1.1/django_timestampable.egg-info/
--rw-r--r--   0 dmp593     (501) staff       (20)    10034 2023-03-04 13:40:53.000000 django-timestampable-1.1.1/django_timestampable.egg-info/PKG-INFO
--rw-r--r--   0 dmp593     (501) staff       (20)      558 2023-03-04 13:40:53.000000 django-timestampable-1.1.1/django_timestampable.egg-info/SOURCES.txt
--rw-r--r--   0 dmp593     (501) staff       (20)        1 2023-03-04 13:40:53.000000 django-timestampable-1.1.1/django_timestampable.egg-info/dependency_links.txt
--rw-r--r--   0 dmp593     (501) staff       (20)       60 2023-03-04 13:40:53.000000 django-timestampable-1.1.1/django_timestampable.egg-info/requires.txt
--rw-r--r--   0 dmp593     (501) staff       (20)       11 2023-03-04 13:40:53.000000 django-timestampable-1.1.1/django_timestampable.egg-info/top_level.txt
--rw-r--r--   0 dmp593     (501) staff       (20)     1309 2023-03-04 13:40:53.759089 django-timestampable-1.1.1/setup.cfg
--rw-r--r--   0 dmp593     (501) staff       (20)      134 2023-03-04 01:00:56.000000 django-timestampable-1.1.1/setup.py
-drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-03-04 13:40:53.757727 django-timestampable-1.1.1/timestamps/
--rw-r--r--   0 dmp593     (501) staff       (20)        0 2022-11-12 11:31:09.000000 django-timestampable-1.1.1/timestamps/__init__.py
--rw-r--r--   0 dmp593     (501) staff       (20)       95 2022-11-12 11:31:09.000000 django-timestampable-1.1.1/timestamps/apps.py
-drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-03-04 13:40:53.758545 django-timestampable-1.1.1/timestamps/drf/
--rw-r--r--   0 dmp593     (501) staff       (20)      371 2023-03-04 01:00:56.000000 django-timestampable-1.1.1/timestamps/drf/__init__.py
--rw-r--r--   0 dmp593     (501) staff       (20)     4705 2023-03-04 01:00:56.000000 django-timestampable-1.1.1/timestamps/drf/mixins.py
--rw-r--r--   0 dmp593     (501) staff       (20)      469 2023-03-04 01:00:56.000000 django-timestampable-1.1.1/timestamps/drf/permissions.py
--rw-r--r--   0 dmp593     (501) staff       (20)     2152 2022-11-12 11:31:09.000000 django-timestampable-1.1.1/timestamps/drf/routers.py
--rw-r--r--   0 dmp593     (501) staff       (20)      414 2023-03-04 01:00:56.000000 django-timestampable-1.1.1/timestamps/drf/utils.py
--rw-r--r--   0 dmp593     (501) staff       (20)      682 2022-11-12 11:31:09.000000 django-timestampable-1.1.1/timestamps/drf/viewsets.py
--rw-r--r--   0 dmp593     (501) staff       (20)      921 2023-03-04 13:18:42.000000 django-timestampable-1.1.1/timestamps/managers.py
--rw-r--r--   0 dmp593     (501) staff       (20)     1720 2023-03-04 13:18:42.000000 django-timestampable-1.1.1/timestamps/models.py
--rw-r--r--   0 dmp593     (501) staff       (20)      613 2022-11-12 11:31:09.000000 django-timestampable-1.1.1/timestamps/querysets.py
--rw-r--r--   0 dmp593     (501) staff       (20)      140 2023-03-04 13:18:42.000000 django-timestampable-1.1.1/timestamps/signals.py
+drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-07-03 09:20:32.696257 django-timestampable-1.1.2/
+-rw-r--r--   0 dmp593     (501) staff       (20)     1063 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/LICENSE
+-rw-r--r--   0 dmp593     (501) staff       (20)       58 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/MANIFEST.in
+-rw-r--r--   0 dmp593     (501) staff       (20)    10073 2023-07-03 09:20:32.696325 django-timestampable-1.1.2/PKG-INFO
+-rw-r--r--   0 dmp593     (501) staff       (20)     8718 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/README.md
+drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-07-03 09:20:32.694454 django-timestampable-1.1.2/django_timestampable.egg-info/
+-rw-r--r--   0 dmp593     (501) staff       (20)    10073 2023-07-03 09:20:32.000000 django-timestampable-1.1.2/django_timestampable.egg-info/PKG-INFO
+-rw-r--r--   0 dmp593     (501) staff       (20)      558 2023-07-03 09:20:32.000000 django-timestampable-1.1.2/django_timestampable.egg-info/SOURCES.txt
+-rw-r--r--   0 dmp593     (501) staff       (20)        1 2023-07-03 09:20:32.000000 django-timestampable-1.1.2/django_timestampable.egg-info/dependency_links.txt
+-rw-r--r--   0 dmp593     (501) staff       (20)       60 2023-07-03 09:20:32.000000 django-timestampable-1.1.2/django_timestampable.egg-info/requires.txt
+-rw-r--r--   0 dmp593     (501) staff       (20)       11 2023-07-03 09:20:32.000000 django-timestampable-1.1.2/django_timestampable.egg-info/top_level.txt
+-rw-r--r--   0 dmp593     (501) staff       (20)     1337 2023-07-03 09:20:32.696610 django-timestampable-1.1.2/setup.cfg
+-rw-r--r--   0 dmp593     (501) staff       (20)      134 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/setup.py
+drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-07-03 09:20:32.695317 django-timestampable-1.1.2/timestamps/
+-rw-r--r--   0 dmp593     (501) staff       (20)        0 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/__init__.py
+-rw-r--r--   0 dmp593     (501) staff       (20)       95 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/apps.py
+drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-07-03 09:20:32.696157 django-timestampable-1.1.2/timestamps/drf/
+-rw-r--r--   0 dmp593     (501) staff       (20)      371 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/drf/__init__.py
+-rw-r--r--   0 dmp593     (501) staff       (20)     4705 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/drf/mixins.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      469 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/drf/permissions.py
+-rw-r--r--   0 dmp593     (501) staff       (20)     2152 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/drf/routers.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      414 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/drf/utils.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      682 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/drf/viewsets.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      921 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/managers.py
+-rw-r--r--   0 dmp593     (501) staff       (20)     1720 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/models.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      613 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/querysets.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      140 2023-07-03 09:16:32.000000 django-timestampable-1.1.2/timestamps/signals.py
```

### Comparing `django-timestampable-1.1.1/LICENSE` & `django-timestampable-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.1/PKG-INFO` & `django-timestampable-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-timestampable
-Version: 1.1.1
+Version: 1.1.2
 Summary: Timestamps and Soft Delete Patterns in Django Models
 Home-page: https://github.com/xgeekshq/django-timestampable/
 Author: Daniel Pinto
 Author-email: dmp593@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-timestampable-1.1.1/README.md` & `django-timestampable-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.1/django_timestampable.egg-info/PKG-INFO` & `django-timestampable-1.1.2/django_timestampable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-timestampable
-Version: 1.1.1
+Version: 1.1.2
 Summary: Timestamps and Soft Delete Patterns in Django Models
 Home-page: https://github.com/xgeekshq/django-timestampable/
 Author: Daniel Pinto
 Author-email: dmp593@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-timestampable-1.1.1/django_timestampable.egg-info/SOURCES.txt` & `django-timestampable-1.1.2/django_timestampable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.1/setup.cfg` & `django-timestampable-1.1.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [metadata]
 name = django-timestampable
-version = 1.1.1
+version = 1.1.2
 description = Timestamps and Soft Delete Patterns in Django Models
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/xgeekshq/django-timestampable/
 author = Daniel Pinto
 author_email = dmp593@gmail.com
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
```

### Comparing `django-timestampable-1.1.1/timestamps/drf/mixins.py` & `django-timestampable-1.1.2/timestamps/drf/mixins.py`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.1/timestamps/drf/routers.py` & `django-timestampable-1.1.2/timestamps/drf/routers.py`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.1/timestamps/drf/viewsets.py` & `django-timestampable-1.1.2/timestamps/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.1/timestamps/managers.py` & `django-timestampable-1.1.2/timestamps/managers.py`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.1/timestamps/models.py` & `django-timestampable-1.1.2/timestamps/models.py`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.1/timestamps/querysets.py` & `django-timestampable-1.1.2/timestamps/querysets.py`

 * *Files identical despite different names*

