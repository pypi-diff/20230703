# Comparing `tmp/django_mongoengine_rql-0.2.1.tar.gz` & `tmp/django_mongoengine_rql-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mongoengine_rql-0.2.1.tar", max compression
+gzip compressed data, was "django_mongoengine_rql-0.2.2.tar", max compression
```

## Comparing `django_mongoengine_rql-0.2.1.tar` & `django_mongoengine_rql-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/LICENSE
--rw-r--r--   0        0        0     3874 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/dj_mongoengine_rql/__init__.py
--rw-r--r--   0        0        0      552 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/dj_mongoengine_rql/constants.py
--rw-r--r--   0        0        0     1752 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/dj_mongoengine_rql/filter_cls.py
--rw-r--r--   0        0        0      322 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/dj_mongoengine_rql/q.py
--rw-r--r--   0        0        0     1965 2023-04-25 09:33:15.985961 django_mongoengine_rql-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5124 1970-01-01 00:00:00.000000 django_mongoengine_rql-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-03 13:35:32.366111 django_mongoengine_rql-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4147 2023-07-03 13:35:32.366111 django_mongoengine_rql-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 13:35:32.370111 django_mongoengine_rql-0.2.2/dj_mongoengine_rql/__init__.py
+-rw-r--r--   0        0        0      552 2023-07-03 13:35:32.370111 django_mongoengine_rql-0.2.2/dj_mongoengine_rql/constants.py
+-rw-r--r--   0        0        0     1752 2023-07-03 13:35:32.370111 django_mongoengine_rql-0.2.2/dj_mongoengine_rql/filter_cls.py
+-rw-r--r--   0        0        0      322 2023-07-03 13:35:32.370111 django_mongoengine_rql-0.2.2/dj_mongoengine_rql/q.py
+-rw-r--r--   0        0        0     2087 2023-07-03 13:36:03.350149 django_mongoengine_rql-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 django_mongoengine_rql-0.2.2/PKG-INFO
```

### Comparing `django_mongoengine_rql-0.2.1/LICENSE` & `django_mongoengine_rql-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_mongoengine_rql-0.2.1/README.md` & `django_mongoengine_rql-0.2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -82,15 +82,18 @@
 * `distinct` setting is not supported for filters
 * annotations are not supported, as well
 
 
 ## Development
 
 1. Python 3.8+
-0. Install dependencies `pip install poetry && poetry install`
+2. Install dependencies `pip install poetry && poetry install`
+3. We use `isort` library to order and format our imports, and `black` - to format the code. 
+   We check it using `flake8-isort` and `flake8-black` libraries (automatically on `flake8` run).  
+   For convenience you may run `docker compose run format` to format the code.
 
 ## Testing
 
 1. Python 3.8+
 0. Install dependencies `pip install poetry && poetry install`
 
 Check code style: `poetry run flake8`
```

### Comparing `django_mongoengine_rql-0.2.1/dj_mongoengine_rql/constants.py` & `django_mongoengine_rql-0.2.2/dj_mongoengine_rql/constants.py`

 * *Files identical despite different names*

### Comparing `django_mongoengine_rql-0.2.1/dj_mongoengine_rql/filter_cls.py` & `django_mongoengine_rql-0.2.2/dj_mongoengine_rql/filter_cls.py`

 * *Files identical despite different names*

### Comparing `django_mongoengine_rql-0.2.1/pyproject.toml` & `django_mongoengine_rql-0.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-mongoengine-rql"
-version = "0.2.1"
+version = "0.2.2"
 description = "Django Mongoengine RQL Filtering"
 authors = ["Ingram Micro"]
 license = "Apache-2.0"
 packages = [
     { include = "dj_mongoengine_rql" }
 ]
 readme = "./README.md"
@@ -34,29 +34,33 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django-rql = "^4.2.0"
 django-mongoengine = "^0.5.4"
 
 [tool.poetry.dev-dependencies]
+urllib3 = "1.*"
+black = "23.*"
 mongoengine = "0.26.*"
 mongomock = "^4.1"
-ipython = "^7.10.0"
+ipython = "^8.10.0"
 pytest = "^7.2.0"
 pytest-cov = "^2.10.1"
 pytest-django = "^4.4"
 pytest-mock = "^3.3.1"
 coverage = {extras = ["toml"], version = "^5.3"}
 flake8 = "~3.8"
+flake8-black = "0.*"
 flake8-bugbear = "~20"
 flake8-cognitive-complexity = "^0.1"
 flake8-commas = "~2.0"
 flake8-future-import = "~0.4"
-flake8-import-order = "~0.18"
+flake8-isort = "5.*"
 flake8-broken-line = "~0.3"
+isort = "5.*"
 Sphinx = "^4.4.0"
 sphinx-rtd-theme = "^1.0.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -72,7 +76,11 @@
 
 [tool.coverage.report]
 omit = []
 
 exclude_lines = [
     "pragma: no cover",
 ]
+
+[tool.black]
+line_length = 100
+skip-string-normalization = true
```

### Comparing `django_mongoengine_rql-0.2.1/PKG-INFO` & `django_mongoengine_rql-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mongoengine-rql
-Version: 0.2.1
+Version: 0.2.2
 Summary: Django Mongoengine RQL Filtering
 Home-page: https://connect.cloudblue.com/community/api/rql/
 License: Apache-2.0
 Keywords: rql,filter,django,mongo,mongoengine
 Author: Ingram Micro
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,17 +15,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Text Processing :: Filters
 Requires-Dist: django-mongoengine (>=0.5.4,<0.6.0)
 Requires-Dist: django-rql (>=4.2.0,<5.0.0)
 Project-URL: Repository, https://github.com/cloudblue/django-mongoengine-rql
 Description-Content-Type: text/markdown
 
 # Django Mongoengine RQL
@@ -112,15 +109,18 @@
 * `distinct` setting is not supported for filters
 * annotations are not supported, as well
 
 
 ## Development
 
 1. Python 3.8+
-0. Install dependencies `pip install poetry && poetry install`
+2. Install dependencies `pip install poetry && poetry install`
+3. We use `isort` library to order and format our imports, and `black` - to format the code. 
+   We check it using `flake8-isort` and `flake8-black` libraries (automatically on `flake8` run).  
+   For convenience you may run `docker compose run format` to format the code.
 
 ## Testing
 
 1. Python 3.8+
 0. Install dependencies `pip install poetry && poetry install`
 
 Check code style: `poetry run flake8`
```

