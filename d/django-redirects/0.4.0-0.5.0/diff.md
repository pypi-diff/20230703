# Comparing `tmp/django-redirects-0.4.0.tar.gz` & `tmp/django-redirects-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-redirects-0.4.0.tar", last modified: Tue Dec 13 22:48:57 2022, max compression
+gzip compressed data, was "django-redirects-0.5.0.tar", last modified: Mon Jul  3 21:48:45 2023, max compression
```

## Comparing `django-redirects-0.4.0.tar` & `django-redirects-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 22:48:57.984848 django-redirects-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2022-12-13 22:48:45.000000 django-redirects-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-13 22:48:45.000000 django-redirects-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2022-12-13 22:48:57.984848 django-redirects-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2022-12-13 22:48:45.000000 django-redirects-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 22:48:57.980848 django-redirects-0.4.0/django_redirects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2022-12-13 22:48:57.000000 django-redirects-0.4.0/django_redirects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      551 2022-12-13 22:48:57.000000 django-redirects-0.4.0/django_redirects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 22:48:57.000000 django-redirects-0.4.0/django_redirects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-13 22:48:57.000000 django-redirects-0.4.0/django_redirects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-13 22:48:45.000000 django-redirects-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 22:48:57.984848 django-redirects-0.4.0/redirects/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 22:48:57.984848 django-redirects-0.4.0/redirects/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/migrations/0002_add_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/migrations/0003_redirect_created_at_redirect_updated_at.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2022-12-13 22:48:45.000000 django-redirects-0.4.0/redirects/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-13 22:48:57.984848 django-redirects-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2022-12-13 22:48:45.000000 django-redirects-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.730301 django-redirects-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-03 21:48:31.000000 django-redirects-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-03 21:48:31.000000 django-redirects-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-07-03 21:48:45.730301 django-redirects-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-03 21:48:31.000000 django-redirects-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.726300 django-redirects-0.5.0/django_redirects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-07-03 21:48:45.000000 django-redirects-0.5.0/django_redirects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-03 21:48:45.000000 django-redirects-0.5.0/django_redirects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:48:45.000000 django-redirects-0.5.0/django_redirects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 21:48:45.000000 django-redirects-0.5.0/django_redirects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-03 21:48:31.000000 django-redirects-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.726300 django-redirects-0.5.0/redirects/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.726300 django-redirects-0.5.0/redirects/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.722300 django-redirects-0.5.0/redirects/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.726300 django-redirects-0.5.0/redirects/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.722300 django-redirects-0.5.0/redirects/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.726300 django-redirects-0.5.0/redirects/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.726300 django-redirects-0.5.0/redirects/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.726300 django-redirects-0.5.0/redirects/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.730301 django-redirects-0.5.0/redirects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/migrations/0002_add_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/migrations/0003_redirect_created_at_redirect_updated_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-03 21:48:31.000000 django-redirects-0.5.0/redirects/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 21:48:45.730301 django-redirects-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 21:48:31.000000 django-redirects-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:48:45.730301 django-redirects-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-03 21:48:31.000000 django-redirects-0.5.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 21:48:31.000000 django-redirects-0.5.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-03 21:48:31.000000 django-redirects-0.5.0/tests/test_models.py
```

### Comparing `django-redirects-0.4.0/LICENSE.txt` & `django-redirects-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-redirects-0.4.0/PKG-INFO` & `django-redirects-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,74 @@
 Metadata-Version: 2.1
 Name: django-redirects
-Version: 0.4.0
+Version: 0.5.0
 Summary: django redirects as they should be, with full control.
-Home-page: https://github.com/fabiocaccamo/django-redirects
-Download-URL: https://github.com/fabiocaccamo/django-redirects/archive/0.4.0.tar.gz
-Author: Fabio Caccamo
-Author-email: fabio.caccamo@gmail.com
+Author-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+Maintainer-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2020-present Fabio Caccamo
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/fabiocaccamo/django-redirects
+Project-URL: Download, https://github.com/fabiocaccamo/django-redirects/releases
 Project-URL: Documentation, https://github.com/fabiocaccamo/django-redirects#readme
 Project-URL: Issues, https://github.com/fabiocaccamo/django-redirects/issues
 Project-URL: Funding, https://github.com/sponsors/fabiocaccamo/
 Project-URL: Twitter, https://twitter.com/fabiocaccamo
 Keywords: django,admin,redirects,redirect,permanent,temporary,301,302,303,307,308,exact,prefix,regex
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
-Requires: django (>= 2.2)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![](https://img.shields.io/pypi/pyversions/django-redirects.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
 [![](https://img.shields.io/pypi/djversions/django-redirects?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
 
 [![](https://img.shields.io/pypi/v/django-redirects.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-redirects/)
 [![](https://pepy.tech/badge/django-redirects/month)](https://pepy.tech/project/django-redirects)
-[![](https://img.shields.io/github/stars/fabiocaccamo/django-redirects?logo=github)](https://github.com/fabiocaccamo/django-redirects/)
-[![](https://img.shields.io/pypi/l/django-redirects.svg?color=blue)](https://github.com/fabiocaccamo/django-redirects/blob/master/LICENSE.txt)
+[![](https://img.shields.io/github/stars/fabiocaccamo/django-redirects?logo=github)](https://github.com/fabiocaccamo/django-redirects/stargazers)
+[![](https://img.shields.io/pypi/l/django-redirects.svg?color=blue)](https://github.com/fabiocaccamo/django-redirects/blob/main/LICENSE.txt)
 
-[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-redirects/master.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-redirects/master)
-[![](https://img.shields.io/github/workflow/status/fabiocaccamo/django-redirects/Test%20package?label=build&logo=github)](https://github.com/fabiocaccamo/django-redirects)
+[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-redirects/main.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-redirects/main)
+[![](https://img.shields.io/github/actions/workflow/status/fabiocaccamo/django-redirects/test-package.yml?branch=main&label=build&logo=github)](https://github.com/fabiocaccamo/django-redirects)
 [![](https://img.shields.io/codecov/c/gh/fabiocaccamo/django-redirects?logo=codecov)](https://codecov.io/gh/fabiocaccamo/django-redirects)
 [![](https://img.shields.io/codacy/grade/6bc31cfdbc2b463b808bd3dc23a44444?logo=codacy)](https://www.codacy.com/app/fabiocaccamo/django-redirects)
 [![](https://img.shields.io/codeclimate/maintainability/fabiocaccamo/django-redirects?logo=code-climate)](https://codeclimate.com/github/fabiocaccamo/django-redirects/)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # django-redirects
 
@@ -81,14 +102,17 @@
 
 # upgrade pip
 python -m pip install --upgrade pip
 
 # install requirements
 pip install -r requirements.txt -r requirements-test.txt
 
+# install pre-commit to run formatters and linters
+pre-commit install --install-hooks
+
 # run tests
 tox
 # or
 python runtests.py
 # or
 python -m django test --settings "tests.settings"
 ```
```

### Comparing `django-redirects-0.4.0/README.md` & `django-redirects-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [![](https://img.shields.io/pypi/pyversions/django-redirects.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
 [![](https://img.shields.io/pypi/djversions/django-redirects?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
 
 [![](https://img.shields.io/pypi/v/django-redirects.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-redirects/)
 [![](https://pepy.tech/badge/django-redirects/month)](https://pepy.tech/project/django-redirects)
-[![](https://img.shields.io/github/stars/fabiocaccamo/django-redirects?logo=github)](https://github.com/fabiocaccamo/django-redirects/)
-[![](https://img.shields.io/pypi/l/django-redirects.svg?color=blue)](https://github.com/fabiocaccamo/django-redirects/blob/master/LICENSE.txt)
+[![](https://img.shields.io/github/stars/fabiocaccamo/django-redirects?logo=github)](https://github.com/fabiocaccamo/django-redirects/stargazers)
+[![](https://img.shields.io/pypi/l/django-redirects.svg?color=blue)](https://github.com/fabiocaccamo/django-redirects/blob/main/LICENSE.txt)
 
-[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-redirects/master.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-redirects/master)
-[![](https://img.shields.io/github/workflow/status/fabiocaccamo/django-redirects/Test%20package?label=build&logo=github)](https://github.com/fabiocaccamo/django-redirects)
+[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-redirects/main.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-redirects/main)
+[![](https://img.shields.io/github/actions/workflow/status/fabiocaccamo/django-redirects/test-package.yml?branch=main&label=build&logo=github)](https://github.com/fabiocaccamo/django-redirects)
 [![](https://img.shields.io/codecov/c/gh/fabiocaccamo/django-redirects?logo=codecov)](https://codecov.io/gh/fabiocaccamo/django-redirects)
 [![](https://img.shields.io/codacy/grade/6bc31cfdbc2b463b808bd3dc23a44444?logo=codacy)](https://www.codacy.com/app/fabiocaccamo/django-redirects)
 [![](https://img.shields.io/codeclimate/maintainability/fabiocaccamo/django-redirects?logo=code-climate)](https://codeclimate.com/github/fabiocaccamo/django-redirects/)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # django-redirects
 
@@ -45,14 +45,17 @@
 
 # upgrade pip
 python -m pip install --upgrade pip
 
 # install requirements
 pip install -r requirements.txt -r requirements-test.txt
 
+# install pre-commit to run formatters and linters
+pre-commit install --install-hooks
+
 # run tests
 tox
 # or
 python runtests.py
 # or
 python -m django test --settings "tests.settings"
 ```
```

### Comparing `django-redirects-0.4.0/django_redirects.egg-info/PKG-INFO` & `django-redirects-0.5.0/django_redirects.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,74 @@
 Metadata-Version: 2.1
 Name: django-redirects
-Version: 0.4.0
+Version: 0.5.0
 Summary: django redirects as they should be, with full control.
-Home-page: https://github.com/fabiocaccamo/django-redirects
-Download-URL: https://github.com/fabiocaccamo/django-redirects/archive/0.4.0.tar.gz
-Author: Fabio Caccamo
-Author-email: fabio.caccamo@gmail.com
+Author-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+Maintainer-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2020-present Fabio Caccamo
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/fabiocaccamo/django-redirects
+Project-URL: Download, https://github.com/fabiocaccamo/django-redirects/releases
 Project-URL: Documentation, https://github.com/fabiocaccamo/django-redirects#readme
 Project-URL: Issues, https://github.com/fabiocaccamo/django-redirects/issues
 Project-URL: Funding, https://github.com/sponsors/fabiocaccamo/
 Project-URL: Twitter, https://twitter.com/fabiocaccamo
 Keywords: django,admin,redirects,redirect,permanent,temporary,301,302,303,307,308,exact,prefix,regex
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
-Requires: django (>= 2.2)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![](https://img.shields.io/pypi/pyversions/django-redirects.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
 [![](https://img.shields.io/pypi/djversions/django-redirects?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
 
 [![](https://img.shields.io/pypi/v/django-redirects.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-redirects/)
 [![](https://pepy.tech/badge/django-redirects/month)](https://pepy.tech/project/django-redirects)
-[![](https://img.shields.io/github/stars/fabiocaccamo/django-redirects?logo=github)](https://github.com/fabiocaccamo/django-redirects/)
-[![](https://img.shields.io/pypi/l/django-redirects.svg?color=blue)](https://github.com/fabiocaccamo/django-redirects/blob/master/LICENSE.txt)
+[![](https://img.shields.io/github/stars/fabiocaccamo/django-redirects?logo=github)](https://github.com/fabiocaccamo/django-redirects/stargazers)
+[![](https://img.shields.io/pypi/l/django-redirects.svg?color=blue)](https://github.com/fabiocaccamo/django-redirects/blob/main/LICENSE.txt)
 
-[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-redirects/master.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-redirects/master)
-[![](https://img.shields.io/github/workflow/status/fabiocaccamo/django-redirects/Test%20package?label=build&logo=github)](https://github.com/fabiocaccamo/django-redirects)
+[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-redirects/main.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-redirects/main)
+[![](https://img.shields.io/github/actions/workflow/status/fabiocaccamo/django-redirects/test-package.yml?branch=main&label=build&logo=github)](https://github.com/fabiocaccamo/django-redirects)
 [![](https://img.shields.io/codecov/c/gh/fabiocaccamo/django-redirects?logo=codecov)](https://codecov.io/gh/fabiocaccamo/django-redirects)
 [![](https://img.shields.io/codacy/grade/6bc31cfdbc2b463b808bd3dc23a44444?logo=codacy)](https://www.codacy.com/app/fabiocaccamo/django-redirects)
 [![](https://img.shields.io/codeclimate/maintainability/fabiocaccamo/django-redirects?logo=code-climate)](https://codeclimate.com/github/fabiocaccamo/django-redirects/)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # django-redirects
 
@@ -81,14 +102,17 @@
 
 # upgrade pip
 python -m pip install --upgrade pip
 
 # install requirements
 pip install -r requirements.txt -r requirements-test.txt
 
+# install pre-commit to run formatters and linters
+pre-commit install --install-hooks
+
 # run tests
 tox
 # or
 python runtests.py
 # or
 python -m django test --settings "tests.settings"
 ```
```

### Comparing `django-redirects-0.4.0/redirects/admin.py` & `django-redirects-0.5.0/redirects/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,19 @@
                 <span style="display: block; white-space: nowrap; font-weight: normal;">
                     <small>{obj.old_path}</small>
                 </span>
                 <span style="display: block; white-space: nowrap;">
                     <span style="color: rgba(0, 0, 0, 0.4);">&searr; {gone}</span> {obj.new_path}
                 </span>
             </span>
-            """.strip()
+            """.strip()  # noqa: E501
         html = mark_safe(html)
         return html
 
     redirect_display.short_description = _("Redirect")
-    redirect_display.allow_tags = True
 
     def test_display(self, obj):
         css = """
             font-weight: normal;
             font-size: 20px;
             line-height: 1em;
             display: inline-block;
@@ -41,15 +40,14 @@
         html = f"""
             <a href="{obj.old_path}" target="_blank" style="{css}">&nearr;</a>
             """.strip()
         html = mark_safe(html)
         return html
 
     test_display.short_description = _("Test")
-    test_display.allow_tags = True
 
     list_display = (
         "redirect_display",
         "match",
         "type_status_code",
         "priority",
         "counter",
```

### Comparing `django-redirects-0.4.0/redirects/middleware.py` & `django-redirects-0.5.0/redirects/middleware.py`

 * *Files identical despite different names*

### Comparing `django-redirects-0.4.0/redirects/migrations/0001_initial.py` & `django-redirects-0.5.0/redirects/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("sites", "0002_alter_domain_unique"),
     ]
 
     operations = [
@@ -23,24 +22,31 @@
                         verbose_name="ID",
                     ),
                 ),
                 (
                     "old_path",
                     models.CharField(
                         db_index=True,
-                        help_text="This can be either an absolute path or a regex (excluding the domain name). ",
+                        help_text=(
+                            "This can be either an absolute path or a regex "
+                            "(excluding the domain name). "
+                        ),
                         max_length=255,
                         verbose_name="Old path",
                     ),
                 ),
                 (
                     "new_path",
                     models.CharField(
                         blank=True,
-                        help_text='This can be either an absolute path, an absolute URL, or a regex. If empty a "410 Gone" response will be returned.',
+                        help_text=(
+                            "This can be either an absolute path, "
+                            "an absolute URL, or a regex. "
+                            'If empty a "410 Gone" response will be returned.'
+                        ),
                         max_length=255,
                         verbose_name="New path",
                     ),
                 ),
                 (
                     "match",
                     models.CharField(
```

### Comparing `django-redirects-0.4.0/redirects/migrations/0002_add_priority.py` & `django-redirects-0.5.0/redirects/migrations/0002_add_priority.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("redirects", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="redirect",
```

### Comparing `django-redirects-0.4.0/redirects/migrations/0003_redirect_created_at_redirect_updated_at.py` & `django-redirects-0.5.0/redirects/migrations/0003_redirect_created_at_redirect_updated_at.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("redirects", "0002_add_priority"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="redirect",
```

### Comparing `django-redirects-0.4.0/redirects/models.py` & `django-redirects-0.5.0/redirects/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 
-from django.conf import settings
 from django.contrib.sites.models import Site
 from django.db import models
 from django.utils.encoding import force_str
 from django.utils.translation import gettext_lazy as _
 
 from redirects.http import (
     HttpResponseGone,
@@ -13,15 +12,14 @@
     HttpResponseStrictPermanentRedirect,
     HttpResponseStrictTemporaryRedirect,
     HttpResponseTemporaryRedirect,
 )
 
 
 class Redirect(models.Model):
-
     TYPE_301 = 301
     TYPE_302 = 302
     TYPE_303 = 303
     TYPE_307 = 307
     TYPE_308 = 308
     TYPE_CHOICES = (
         (TYPE_301, _("301 - Permanent")),
@@ -53,15 +51,16 @@
     )
 
     old_path = models.CharField(
         db_index=True,
         max_length=255,
         verbose_name=_("Old path"),
         help_text=_(
-            "This can be either an absolute path or a regex (excluding the domain name). "
+            "This can be either an absolute path or a regex "
+            "(excluding the domain name). "
         ),
     )
 
     new_path = models.CharField(
         max_length=255,
         blank=True,
         verbose_name=_("New path"),
@@ -172,9 +171,10 @@
         unique_together = [["site", "old_path"]]
         verbose_name = _("Redirect")
         verbose_name_plural = _("Redirects")
 
     def __str__(self):
         verbose_name = _("Redirect")
         return force_str(
-            f"{verbose_name} {self.type_status_code}: {self.old_path} \n---> {self.new_path}"
+            f"{verbose_name} {self.type_status_code}: "
+            f"{self.old_path} \n---> {self.new_path}"
         )
```

### Comparing `django-redirects-0.4.0/setup.py` & `django-redirects-0.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,102 @@
-#!/usr/bin/env python
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "django-redirects"
+description = "django redirects as they should be, with full control."
+authors = [
+    { name = "Fabio Caccamo", email = "fabio.caccamo@gmail.com" },
+]
+keywords = [
+    "django",
+    "admin",
+    "redirects",
+    "redirect",
+    "permanent",
+    "temporary",
+    "301",
+    "302",
+    "303",
+    "307",
+    "308",
+    "exact",
+    "prefix",
+    "regex",
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Web Environment",
+    "Framework :: Django",
+    "Framework :: Django :: 3.0",
+    "Framework :: Django :: 3.1",
+    "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Build Tools",
+]
+dynamic = ["version"]
+maintainers = [
+    { name = "Fabio Caccamo", email = "fabio.caccamo@gmail.com" },
+]
+
+[project.readme]
+file = "README.md"
+content-type = "text/markdown"
+
+[project.license]
+file = "LICENSE.txt"
+content-type = "text/plain"
+
+[project.urls]
+Homepage = "https://github.com/fabiocaccamo/django-redirects"
+Download = "https://github.com/fabiocaccamo/django-redirects/releases"
+Documentation = "https://github.com/fabiocaccamo/django-redirects#readme"
+Issues = "https://github.com/fabiocaccamo/django-redirects/issues"
+Funding = "https://github.com/sponsors/fabiocaccamo/"
+Twitter = "https://twitter.com/fabiocaccamo"
+
+[tool.black]
+line-length = 88
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | _build
+  | buck-out
+  | build
+  | dist
+  | venv
+)/
+'''
+
+[tool.isort]
+profile = "black"
+
+[tool.ruff]
+ignore = []
+line-length = 88
+select = ["B", "B9", "C", "E", "F", "W"]
 
-import os
-import sys
+[tool.ruff.mccabe]
+max-complexity = 10
 
-from setuptools import find_packages, setup
+[tool.setuptools.packages.find]
+include = ["redirects*"]
 
-exec(open("redirects/metadata.py").read())
-
-package_name = "django-redirects"
-package_url = f"https://github.com/fabiocaccamo/{package_name}"
-package_path = os.path.abspath(os.path.dirname(__file__))
-download_url = f"{package_url}/archive/{__version__}.tar.gz"
-documentation_url = f"{package_url}#readme"
-issues_url = f"{package_url}/issues"
-sponsor_url = "https://github.com/sponsors/fabiocaccamo/"
-twitter_url = "https://twitter.com/fabiocaccamo"
-
-long_description_file_path = os.path.join(package_path, "README.md")
-long_description_content_type = "text/markdown"
-long_description = ""
-try:
-    with open(long_description_file_path, "r", encoding="utf-8") as f:
-        long_description = f.read()
-except IOError:
-    pass
-
-setup(
-    name=package_name,
-    packages=find_packages(exclude=["contrib", "docs", "tests*"]),
-    include_package_data=True,
-    version=__version__,
-    description=__description__,
-    long_description=long_description,
-    long_description_content_type=long_description_content_type,
-    author=__author__,
-    author_email=__email__,
-    url=package_url,
-    download_url=download_url,
-    project_urls={
-        "Documentation": documentation_url,
-        "Issues": issues_url,
-        "Funding": sponsor_url,
-        "Twitter": twitter_url,
-    },
-    keywords=[
-        "django",
-        "admin",
-        "redirects",
-        "redirect",
-        "permanent",
-        "temporary",
-        "301",
-        "302",
-        "303",
-        "307",
-        "308",
-        "exact",
-        "prefix",
-        "regex",
-    ],
-    requires=[
-        "django (>= 2.2)",
-    ],
-    install_requires=[],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Web Environment",
-        "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
-        "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
-        "Framework :: Django :: 4.1",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Topic :: Software Development :: Build Tools",
-    ],
-)
+[tool.setuptools.dynamic.version]
+attr = "redirects.metadata.__version__"
```

