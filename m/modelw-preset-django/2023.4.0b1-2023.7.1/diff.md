# Comparing `tmp/modelw_preset_django-2023.4.0b1.tar.gz` & `tmp/modelw_preset_django-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_preset_django-2023.4.0b1.tar", max compression
+gzip compressed data, was "modelw_preset_django-2023.7.1.tar", max compression
```

## Comparing `modelw_preset_django-2023.4.0b1.tar` & `modelw_preset_django-2023.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      484 2023-05-04 14:54:08.716745 modelw_preset_django-2023.4.0b1/LICENSE
--rw-r--r--   0        0        0      277 2023-05-04 14:54:08.716745 modelw_preset_django-2023.4.0b1/README.md
--rw-r--r--   0        0        0     1903 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/pyproject.toml
--rw-r--r--   0        0        0    29199 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/__init__.py
--rw-r--r--   0        0        0      400 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/drf.py
--rw-r--r--   0        0        0        0 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/management/commands/__init__.py
--rw-r--r--   0        0        0     2994 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py
--rw-r--r--   0        0        0        0 2023-05-04 14:54:08.720745 modelw_preset_django-2023.4.0b1/src/model_w/preset/django/py.typed
--rw-r--r--   0        0        0     2297 1970-01-01 00:00:00.000000 modelw_preset_django-2023.4.0b1/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-07-03 18:16:39.809140 modelw_preset_django-2023.7.1/LICENSE
+-rw-r--r--   0        0        0      277 2023-07-03 18:16:39.809140 modelw_preset_django-2023.7.1/README.md
+-rw-r--r--   0        0        0     1893 2023-07-03 18:16:39.813140 modelw_preset_django-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0    29199 2023-07-03 18:16:39.813140 modelw_preset_django-2023.7.1/src/model_w/preset/django/__init__.py
+-rw-r--r--   0        0        0      400 2023-07-03 18:16:39.813140 modelw_preset_django-2023.7.1/src/model_w/preset/django/drf.py
+-rw-r--r--   0        0        0        0 2023-07-03 18:16:39.813140 modelw_preset_django-2023.7.1/src/model_w/preset/django/env_helper/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 18:16:39.813140 modelw_preset_django-2023.7.1/src/model_w/preset/django/env_helper/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 18:16:39.813140 modelw_preset_django-2023.7.1/src/model_w/preset/django/env_helper/management/commands/__init__.py
+-rw-r--r--   0        0        0     2994 2023-07-03 18:16:39.813140 modelw_preset_django-2023.7.1/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py
+-rw-r--r--   0        0        0        0 2023-07-03 18:16:39.813140 modelw_preset_django-2023.7.1/src/model_w/preset/django/py.typed
+-rw-r--r--   0        0        0     2281 1970-01-01 00:00:00.000000 modelw_preset_django-2023.7.1/PKG-INFO
```

### Comparing `modelw_preset_django-2023.4.0b1/pyproject.toml` & `modelw_preset_django-2023.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-preset-django"
-version = "2023.4.0b1"
+version = "2023.7.1"
 packages = [
     {  include = "model_w/preset/django", from = "src" }
 ]
 
 description = "Model W preset for Django"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
@@ -19,36 +19,36 @@
 
 repository = "https://github.com/ModelW/preset-django"
 homepage = "https://github.com/ModelW/preset-django"
 
 keywords = ["django", "env", "configuration"]
 
 [tool.poetry.dependencies]
-python = '~3.10'
+python = '~3.11'
 setuptools = "*"
-Django = {version = "~4.1", extras = ["argon2"]}
-sentry-sdk = "~1.18"
-modelw-env-manager = "~1.0.0b2"
+django = {version = "~4.1", extras = ["argon2"]}
+sentry-sdk = "~1.26"
+modelw-env-manager = "~1.0"
 coloredlogs = "~15.0"
-dj-database-url = "~1.3"
+dj-database-url = "~2.0"
 django-postgres-extra = "~2.0"
-whitenoise = "~6.4"
+whitenoise = "~6.5"
 psycopg2 = "~2.9"
-rich = "~13.3"
+rich = "~13.4"
 django-wailer = "~1.0.0-beta.2"
 djangorestframework = "~3.14"
 djangorestframework-gis = "~1.0"
-celery = {extras = ["redis", "tblib"], version = "~5.2", optional = true}
-django-celery-results = {version = "~2.4", optional = true}
-channels = {version = "~4.0.0", extras = ["daphne"], optional = true}
-channels-redis = {version = "~4.0.0", optional = true}
-wagtail = {version = "~4.1", optional = true}
+celery = {extras = ["redis", "tblib"], version = "~5.3", optional = true}
+django-celery-results = {version = "~2.5", optional = true}
+channels = {version = "~4.0", extras = ["daphne"], optional = true}
+channels-redis = {version = "~4.0", optional = true}
+wagtail = {version = "~4.2", optional = true}
 wand = {version = "~0.6", optional = true}
 django-storages = {version = "~1.13", optional = true}
-boto3 = {version = "~1.24", optional = true}
+boto3 = {version = "~1.26", optional = true}
 gunicorn = {version = "~20.1", optional = true}
 
 [tool.poetry.dev-dependencies]
 isort = "*"
 black = "*"
 
 [tool.poetry.extras]
```

### Comparing `modelw_preset_django-2023.4.0b1/src/model_w/preset/django/__init__.py` & `modelw_preset_django-2023.7.1/src/model_w/preset/django/__init__.py`

 * *Files identical despite different names*

### Comparing `modelw_preset_django-2023.4.0b1/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py` & `modelw_preset_django-2023.7.1/src/model_w/preset/django/env_helper/management/commands/list_used_env_vars.py`

 * *Files identical despite different names*

### Comparing `modelw_preset_django-2023.4.0b1/PKG-INFO` & `modelw_preset_django-2023.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: modelw-preset-django
-Version: 2023.4.0b1
+Version: 2023.7.1
 Summary: Model W preset for Django
 Home-page: https://github.com/ModelW/preset-django
 License: WTFPL
 Keywords: django,env,configuration
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: celery
 Provides-Extra: channels
 Provides-Extra: gunicorn
 Provides-Extra: storages
 Provides-Extra: wagtail
-Requires-Dist: Django[argon2] (>=4.1,<4.2)
-Requires-Dist: boto3 (>=1.24,<1.25) ; extra == "wagtail" or extra == "storages"
-Requires-Dist: celery[redis,tblib] (>=5.2,<5.3) ; extra == "celery"
-Requires-Dist: channels-redis (>=4.0.0,<4.1.0) ; extra == "channels"
-Requires-Dist: channels[daphne] (>=4.0.0,<4.1.0) ; extra == "channels"
+Requires-Dist: boto3 (>=1.26,<1.27) ; extra == "wagtail" or extra == "storages"
+Requires-Dist: celery[redis,tblib] (>=5.3,<5.4) ; extra == "celery"
+Requires-Dist: channels-redis (>=4.0,<4.1) ; extra == "channels"
+Requires-Dist: channels[daphne] (>=4.0,<4.1) ; extra == "channels"
 Requires-Dist: coloredlogs (>=15.0,<15.1)
-Requires-Dist: dj-database-url (>=1.3,<1.4)
-Requires-Dist: django-celery-results (>=2.4,<2.5) ; extra == "celery"
+Requires-Dist: dj-database-url (>=2.0,<2.1)
+Requires-Dist: django-celery-results (>=2.5,<2.6) ; extra == "celery"
 Requires-Dist: django-postgres-extra (>=2.0,<2.1)
 Requires-Dist: django-storages (>=1.13,<1.14) ; extra == "wagtail" or extra == "storages"
 Requires-Dist: django-wailer (>=1.0.0-beta.2,<1.1.0)
+Requires-Dist: django[argon2] (>=4.1,<4.2)
 Requires-Dist: djangorestframework (>=3.14,<3.15)
 Requires-Dist: djangorestframework-gis (>=1.0,<1.1)
 Requires-Dist: gunicorn (>=20.1,<20.2) ; extra == "gunicorn"
-Requires-Dist: modelw-env-manager (>=1.0.0b2,<1.1.0)
+Requires-Dist: modelw-env-manager (>=1.0,<1.1)
 Requires-Dist: psycopg2 (>=2.9,<2.10)
-Requires-Dist: rich (>=13.3,<13.4)
-Requires-Dist: sentry-sdk (>=1.18,<1.19)
+Requires-Dist: rich (>=13.4,<13.5)
+Requires-Dist: sentry-sdk (>=1.26,<1.27)
 Requires-Dist: setuptools
-Requires-Dist: wagtail (>=4.1,<4.2) ; extra == "wagtail"
+Requires-Dist: wagtail (>=4.2,<4.3) ; extra == "wagtail"
 Requires-Dist: wand (>=0.6,<0.7) ; extra == "wagtail"
-Requires-Dist: whitenoise (>=6.4,<6.5)
+Requires-Dist: whitenoise (>=6.5,<6.6)
 Project-URL: Repository, https://github.com/ModelW/preset-django
 Description-Content-Type: text/markdown
 
 # Model W &mdash; Django Preset
 
 This Django preset for Model W's Env Manager provides a basic Django
 configuration that is fit to work in PaaS platforms such as DigitalOcean's PaaS.
```

