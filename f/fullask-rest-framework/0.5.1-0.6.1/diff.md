# Comparing `tmp/fullask_rest_framework-0.5.1.tar.gz` & `tmp/fullask_rest_framework-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullask_rest_framework-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fullask_rest_framework-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fullask_rest_framework-0.5.1.tar` & `fullask_rest_framework-0.6.1.tar`

### file list

```diff
@@ -1,53 +1,51 @@
--rw-r--r--   0        0        0      292 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/.editorconfig
--rw-r--r--   0        0        0     1226 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/.gitignore
--rw-r--r--   0        0        0     1070 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/LICENSE
--rw-r--r--   0        0        0     3351 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/README.md
--rw-r--r--   0        0        0      150 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/__init__.py
--rw-r--r--   0        0        0      604 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/cli.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/index.html
--rw-r--r--   0        0        0      851 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/login_form.html
--rw-r--r--   0        0        0     1146 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
--rw-r--r--   0        0        0      202 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/views.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/app_template/__init__.txt
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/app_template/models.txt
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/app_template/resources.txt
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/app_template/schemas.txt
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/__init__.txt
--rw-r--r--   0        0        0      112 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/app.txt
--rw-r--r--   0        0        0      322 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/config.py.txt
--rw-r--r--   0        0        0      628 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/factory.txt
--rw-r--r--   0        0        0       65 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/tests.txt
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/entities/__init__.py
--rw-r--r--   0        0        0       49 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/entities/base_entity.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/__init__.py
--rw-r--r--   0        0        0     6242 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/app_factory.py
--rw-r--r--   0        0        0      104 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/exceptions.py
--rw-r--r--   0        0        0      683 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/extensions.py
--rw-r--r--   0        0        0      206 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/microapp.py
--rw-r--r--   0        0        0       46 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/factory/warnings.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/orm/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/orm/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      292 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/orm/sqlalchemy/base_model.py
--rw-r--r--   0        0        0     1004 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/orm/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/__init__.py
--rw-r--r--   0        0        0      243 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/base.py
--rw-r--r--   0        0        0     2821 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/crud.py
--rw-r--r--   0        0        0     8865 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.306545 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/__init__.py
--rw-r--r--   0        0        0     1212 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/fields.py
--rw-r--r--   0        0        0      261 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/filtering.py
--rw-r--r--   0        0        0     1014 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/pagination.py
--rw-r--r--   0        0        0      644 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/sorting.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/utils/__init__.py
--rw-r--r--   0        0        0      572 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/utils/jwt.py
--rw-r--r--   0        0        0      138 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/vo/__init__.py
--rw-r--r--   0        0        0      346 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/vo/filtering.py
--rw-r--r--   0        0        0      450 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/vo/pagination.py
--rw-r--r--   0        0        0      407 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/fullask_rest_framework/vo/sorting.py
--rw-r--r--   0        0        0     2267 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      316 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/setup.cfg
--rw-r--r--   0        0        0      213 2023-07-01 18:10:54.310546 fullask_rest_framework-0.5.1/tox.ini
--rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 fullask_rest_framework-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      292 2023-07-03 09:50:52.204929 fullask_rest_framework-0.6.1/.editorconfig
+-rw-r--r--   0        0        0     1240 2023-07-03 09:50:52.204929 fullask_rest_framework-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1070 2023-07-03 09:50:52.204929 fullask_rest_framework-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3359 2023-07-03 09:50:52.204929 fullask_rest_framework-0.6.1/README.md
+-rw-r--r--   0        0        0      150 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/__init__.py
+-rw-r--r--   0        0        0      604 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/cli.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/index.html
+-rw-r--r--   0        0        0      851 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/login_form.html
+-rw-r--r--   0        0        0     1146 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
+-rw-r--r--   0        0        0      202 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/views.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/app_template/__init__.txt
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/app_template/models.txt
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/app_template/resources.txt
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/app_template/schemas.txt
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/__init__.txt
+-rw-r--r--   0        0        0      112 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/app.txt
+-rw-r--r--   0        0        0      322 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/config.py.txt
+-rw-r--r--   0        0        0      628 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/factory.txt
+-rw-r--r--   0        0        0       65 2023-07-03 09:50:52.208930 fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/tests.txt
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/db/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/db/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/db/sqlalchemy/base_model.py
+-rw-r--r--   0        0        0     1004 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/db/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/__init__.py
+-rw-r--r--   0        0        0     6242 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/app_factory.py
+-rw-r--r--   0        0        0      104 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/exceptions.py
+-rw-r--r--   0        0        0      683 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/extensions.py
+-rw-r--r--   0        0        0      206 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/microapp.py
+-rw-r--r--   0        0        0       46 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/factory/warnings.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/__init__.py
+-rw-r--r--   0        0        0      157 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/base.py
+-rw-r--r--   0        0        0     2821 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/crud.py
+-rw-r--r--   0        0        0     5952 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/__init__.py
+-rw-r--r--   0        0        0     1212 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/fields.py
+-rw-r--r--   0        0        0      261 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/filtering.py
+-rw-r--r--   0        0        0     1014 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/pagination.py
+-rw-r--r--   0        0        0      644 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/sorting.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/utils/__init__.py
+-rw-r--r--   0        0        0      572 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/utils/jwt.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/vo/__init__.py
+-rw-r--r--   0        0        0      346 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/vo/filtering.py
+-rw-r--r--   0        0        0      364 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/vo/pagination.py
+-rw-r--r--   0        0        0      407 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/fullask_rest_framework/vo/sorting.py
+-rw-r--r--   0        0        0     2267 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      317 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/setup.cfg
+-rw-r--r--   0        0        0      213 2023-07-03 09:50:52.212930 fullask_rest_framework-0.6.1/tox.ini
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 fullask_rest_framework-0.6.1/PKG-INFO
```

### Comparing `fullask_rest_framework-0.5.1/.gitignore` & `fullask_rest_framework-0.6.1/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/apidocs/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `fullask_rest_framework-0.5.1/LICENSE` & `fullask_rest_framework-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/README.md` & `fullask_rest_framework-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 </div>
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/tgoddessana/flask-rest-framework">
-    <img src="docs/frf-logo.png" style="width:75%";>
+    <img src="docs/_static/frf-logo.png" style="width:75%";>
   </a>
 
 <h3 align="center">Fullask-REST-Framework</h3>
 
   <p align="center">
     A fully-supported flask extension to build REST API.
     <br />
```

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/cli.py` & `fullask_rest_framework-0.6.1/fullask_rest_framework/cli.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/login_form.html` & `fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css` & `fullask_rest_framework-0.6.1/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/createproject_template/project_template/factory.txt` & `fullask_rest_framework-0.6.1/fullask_rest_framework/createproject_template/project_template/factory.txt`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/factory/app_factory.py` & `fullask_rest_framework-0.6.1/fullask_rest_framework/factory/app_factory.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/factory/extensions.py` & `fullask_rest_framework-0.6.1/fullask_rest_framework/factory/extensions.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/orm/sqlalchemy/mixins.py` & `fullask_rest_framework-0.6.1/fullask_rest_framework/db/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/repositories/crud.py` & `fullask_rest_framework-0.6.1/fullask_rest_framework/repositories/crud.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/fields.py` & `fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/pagination.py` & `fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/schemas/sorting.py` & `fullask_rest_framework-0.6.1/fullask_rest_framework/schemas/sorting.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/fullask_rest_framework/utils/jwt.py` & `fullask_rest_framework-0.6.1/fullask_rest_framework/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `fullask_rest_framework-0.5.1/pyproject.toml` & `fullask_rest_framework-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "docs/",
     "tests/",
     ".github/"
 ]
 
 [tool.poetry]
 name = "fullask-rest-framework"
-version = "0.5.1"
+version = "0.6.1"
 description = ""
 authors = ["tgoddessana <twicegoddessana1229@gmail.com>"]
 
 [tool.poetry.dependencies]
 pip = "*"
 python = "^3.11"
 flask = "^2.2.3"
@@ -76,15 +76,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 wheel = "^0.40.0"
 twine = "^4.0.2"
 pre-commit = "^3.3.2"
-bumpversion = "^0.6.0"
+bumpversion = "^0.6.1"
 flit = "^3.9.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 flake8 = "^6.0.0"
 tox = "*"
```

### Comparing `fullask_rest_framework-0.5.1/PKG-INFO` & `fullask_rest_framework-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullask-rest-framework
-Version: 0.5.1
+Version: 0.6.1
 Summary: A fully-supported flask extension to build REST API.
 Author-email: tgoddessana <twicegoddessana1229@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,15 @@
 </div>
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/tgoddessana/flask-rest-framework">
-    <img src="docs/frf-logo.png" style="width:75%";>
+    <img src="docs/_static/frf-logo.png" style="width:75%";>
   </a>
 
 <h3 align="center">Fullask-REST-Framework</h3>
 
   <p align="center">
     A fully-supported flask extension to build REST API.
     <br />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.5.1 Summary: A
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.6.1 Summary: A
 fully-supported flask extension to build REST API. Author-email: tgoddessana
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

