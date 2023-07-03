# Comparing `tmp/django-translator-1.1.0b2.tar.gz` & `tmp/django-translator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-translator-1.1.0b2.tar", last modified: Thu Jul 28 14:53:49 2022, max compression
+gzip compressed data, was "django-translator-1.1.1.tar", last modified: Mon Jul  3 13:39:52 2023, max compression
```

## Comparing `django-translator-1.1.0b2.tar` & `django-translator-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,41 @@
-drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2022-07-28 14:53:49.495713 django-translator-1.1.0b2/
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1078 2018-09-17 06:38:48.000000 django-translator-1.1.0b2/LICENSE
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       65 2018-09-17 06:38:48.000000 django-translator-1.1.0b2/MANIFEST.in
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     4545 2022-07-28 14:53:49.495506 django-translator-1.1.0b2/PKG-INFO
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     3849 2022-07-28 14:08:01.000000 django-translator-1.1.0b2/README.rst
-drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2022-07-28 14:53:49.493213 django-translator-1.1.0b2/django_translator.egg-info/
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     4545 2022-07-28 14:53:49.000000 django-translator-1.1.0b2/django_translator.egg-info/PKG-INFO
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      464 2022-07-28 14:53:49.000000 django-translator-1.1.0b2/django_translator.egg-info/SOURCES.txt
--rw-r--r--   0 samuelbichsel   (501) staff       (20)        1 2022-07-28 14:53:49.000000 django-translator-1.1.0b2/django_translator.egg-info/dependency_links.txt
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       65 2022-07-28 14:53:49.000000 django-translator-1.1.0b2/django_translator.egg-info/requires.txt
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       11 2022-07-28 14:53:49.000000 django-translator-1.1.0b2/django_translator.egg-info/top_level.txt
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       38 2022-07-28 14:53:49.495783 django-translator-1.1.0b2/setup.cfg
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1175 2022-07-28 14:53:25.000000 django-translator-1.1.0b2/setup.py
-drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2022-07-28 14:53:49.494618 django-translator-1.1.0b2/translator/
--rw-r--r--   0 samuelbichsel   (501) staff       (20)        0 2018-09-17 06:38:48.000000 django-translator-1.1.0b2/translator/__init__.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1300 2022-07-28 14:51:51.000000 django-translator-1.1.0b2/translator/admin.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      873 2022-07-28 09:20:34.000000 django-translator-1.1.0b2/translator/context_processors.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1128 2022-07-28 14:52:18.000000 django-translator-1.1.0b2/translator/models.py
-drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2022-07-28 14:53:49.495231 django-translator-1.1.0b2/translator/templatetags/
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       23 2018-09-17 06:38:48.000000 django-translator-1.1.0b2/translator/templatetags/__init__.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      734 2022-07-28 09:20:34.000000 django-translator-1.1.0b2/translator/templatetags/translator_tags.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      292 2022-07-28 09:20:34.000000 django-translator-1.1.0b2/translator/translation.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     2744 2022-07-28 14:51:08.000000 django-translator-1.1.0b2/translator/util.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 13:39:52.306347 django-translator-1.1.1/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1078 2020-01-22 15:12:27.000000 django-translator-1.1.1/LICENSE
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       65 2020-01-22 15:12:27.000000 django-translator-1.1.1/MANIFEST.in
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     4544 2023-07-03 13:39:52.306088 django-translator-1.1.1/PKG-INFO
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     3849 2022-11-10 14:44:42.000000 django-translator-1.1.1/README.rst
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 13:39:52.290518 django-translator-1.1.1/django_translator.egg-info/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     4544 2023-07-03 13:39:52.000000 django-translator-1.1.1/django_translator.egg-info/PKG-INFO
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1290 2023-07-03 13:39:52.000000 django-translator-1.1.1/django_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        1 2023-07-03 13:39:52.000000 django-translator-1.1.1/django_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       65 2023-07-03 13:39:52.000000 django-translator-1.1.1/django_translator.egg-info/requires.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       11 2023-07-03 13:39:52.000000 django-translator-1.1.1/django_translator.egg-info/top_level.txt
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       38 2023-07-03 13:39:52.306438 django-translator-1.1.1/setup.cfg
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1173 2023-07-03 13:31:55.000000 django-translator-1.1.1/setup.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 13:39:52.293889 django-translator-1.1.1/translator/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)        0 2020-01-22 15:12:27.000000 django-translator-1.1.1/translator/__init__.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 13:39:52.301603 django-translator-1.1.1/translator/__pycache__/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      181 2020-01-22 15:14:23.000000 django-translator-1.1.1/translator/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      181 2021-09-01 09:51:27.000000 django-translator-1.1.1/translator/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2095 2020-01-24 14:57:22.000000 django-translator-1.1.1/translator/__pycache__/admin.cpython-38.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2085 2021-09-01 09:51:28.000000 django-translator-1.1.1/translator/__pycache__/admin.cpython-39.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      821 2020-01-22 15:14:25.000000 django-translator-1.1.1/translator/__pycache__/context_processors.cpython-38.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1224 2021-09-02 11:15:57.000000 django-translator-1.1.1/translator/__pycache__/context_processors.cpython-39.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1397 2020-01-22 15:14:23.000000 django-translator-1.1.1/translator/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2022 2021-09-02 11:15:57.000000 django-translator-1.1.1/translator/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      557 2020-01-22 15:14:23.000000 django-translator-1.1.1/translator/__pycache__/translation.cpython-38.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      557 2021-09-01 09:51:28.000000 django-translator-1.1.1/translator/__pycache__/translation.cpython-39.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1889 2020-01-22 15:14:23.000000 django-translator-1.1.1/translator/__pycache__/util.cpython-38.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2478 2021-09-02 11:15:57.000000 django-translator-1.1.1/translator/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1300 2022-11-10 14:44:42.000000 django-translator-1.1.1/translator/admin.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      873 2021-09-02 11:15:56.000000 django-translator-1.1.1/translator/context_processors.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1128 2022-11-10 14:44:42.000000 django-translator-1.1.1/translator/models.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 13:39:52.303107 django-translator-1.1.1/translator/templatetags/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)       23 2020-01-22 15:12:27.000000 django-translator-1.1.1/translator/templatetags/__init__.py
+drwxr-xr-x   0 christianschuermann   (501) staff       (20)        0 2023-07-03 13:39:52.305455 django-translator-1.1.1/translator/templatetags/__pycache__/
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      194 2020-01-22 15:14:23.000000 django-translator-1.1.1/translator/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      194 2021-09-01 09:51:29.000000 django-translator-1.1.1/translator/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1179 2020-01-22 15:14:23.000000 django-translator-1.1.1/translator/templatetags/__pycache__/translator_tags.cpython-38.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     1179 2021-09-01 09:51:29.000000 django-translator-1.1.1/translator/templatetags/__pycache__/translator_tags.cpython-39.pyc
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      734 2020-01-22 15:12:27.000000 django-translator-1.1.1/translator/templatetags/translator_tags.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)      292 2020-01-22 15:12:27.000000 django-translator-1.1.1/translator/translation.py
+-rw-r--r--   0 christianschuermann   (501) staff       (20)     2698 2023-07-03 13:34:40.000000 django-translator-1.1.1/translator/util.py
```

### Comparing `django-translator-1.1.0b2/LICENSE` & `django-translator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-translator-1.1.0b2/PKG-INFO` & `django-translator-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-translator
-Version: 1.1.0b2
+Version: 1.1.1
 Summary: Translator is an app for collecting translations for specified keys in django admin.
-Home-page: http://www.dreipol.ch/
+Home-page: https://www.dreipol.ch/
 Author: dreipol GmbH
 Author-email: dev@dreipol.ch
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-translator-1.1.0b2/README.rst` & `django-translator-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-translator-1.1.0b2/django_translator.egg-info/PKG-INFO` & `django-translator-1.1.1/django_translator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-translator
-Version: 1.1.0b2
+Version: 1.1.1
 Summary: Translator is an app for collecting translations for specified keys in django admin.
-Home-page: http://www.dreipol.ch/
+Home-page: https://www.dreipol.ch/
 Author: dreipol GmbH
 Author-email: dev@dreipol.ch
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-translator-1.1.0b2/setup.py` & `django-translator-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 reqs = ['Django>=3.2', 'django-modeltranslation>=0.18.4', 'django-taggit>= 2.0.0']
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-translator',
-    version='1.1.0-b2',
+    version='1.1.1',
     packages=['translator'],
     include_package_data=True,
     license='MIT License',
     description='Translator is an app for collecting translations for specified keys in django admin.',
     long_description=README,
-    url='http://www.dreipol.ch/',
+    url='https://www.dreipol.ch/',
     author='dreipol GmbH',
     author_email='dev@dreipol.ch',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',  # example license
```

### Comparing `django-translator-1.1.0b2/translator/admin.py` & `django-translator-1.1.1/translator/admin.py`

 * *Files identical despite different names*

### Comparing `django-translator-1.1.0b2/translator/context_processors.py` & `django-translator-1.1.1/translator/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-translator-1.1.0b2/translator/models.py` & `django-translator-1.1.1/translator/models.py`

 * *Files identical despite different names*

### Comparing `django-translator-1.1.0b2/translator/templatetags/translator_tags.py` & `django-translator-1.1.1/translator/templatetags/translator_tags.py`

 * *Files identical despite different names*

### Comparing `django-translator-1.1.0b2/translator/util.py` & `django-translator-1.1.1/translator/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 from django.utils.functional import lazy
 from django.utils.module_loading import import_string
 from django.utils.safestring import mark_safe
 
 from translator.context_processors import DJANGO_TRANSLATOR_MODELS
 
 CACHE_TIMEOUT = getattr(settings, "DJANGO_TRANSLATOR_CACHE_TIMEOUT", DEFAULT_TIMEOUT)
-TRANSLATOR_IS_ENABLED = getattr(settings, "DJANGO_TRANSLATOR_ENABLED", True)
 
 
 def get_translation_for_key(item, model_class=None):
     from django.core.cache import cache
     from django.core.exceptions import ObjectDoesNotExist
     from django.utils.translation import get_language
 
     from translator.models import Translation
 
-    if TRANSLATOR_IS_ENABLED:
+    if getattr(settings, "DJANGO_TRANSLATOR_ENABLED", True):
         if not model_class:
             model_class = Translation  # We are using the Translation model as default
 
         lang = get_language()
         key = get_key(lang, item, model_class.cache_key_prefix)
         result = cache.get(key)
```

