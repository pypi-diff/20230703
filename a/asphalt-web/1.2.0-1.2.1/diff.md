# Comparing `tmp/asphalt-web-1.2.0.tar.gz` & `tmp/asphalt-web-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asphalt-web-1.2.0.tar", last modified: Fri Jun 30 17:30:17 2023, max compression
+gzip compressed data, was "asphalt-web-1.2.1.tar", last modified: Mon Jul  3 09:26:38 2023, max compression
```

## Comparing `asphalt-web-1.2.0.tar` & `asphalt-web-1.2.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.129054 asphalt-web-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-30 17:30:17.129054 asphalt-web-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/integrations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/asgi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/django.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/fastapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/modules/starlette.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/py-modindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/docs/versionhistory.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/aiohttp/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/aiohttp/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/aiohttp/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/aiohttp/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/asgi3/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/asgi3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/asgi3/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/asgi3/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/django/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/django/django_example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/django_example/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/django/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.117054 asphalt-web-1.2.0/examples/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/fastapi/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/fastapi/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/fastapi/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/fastapi/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.121054 asphalt-web-1.2.0/examples/starlette/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/starlette/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/starlette/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/starlette/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/examples/starlette/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:30:17.129054 asphalt-web-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.113054 asphalt-web-1.2.0/src/asphalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.121054 asphalt-web-1.2.0/src/asphalt/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/asgi3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/src/asphalt/web/starlette.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.125054 asphalt-web-1.2.0/src/asphalt_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 17:30:17.000000 asphalt-web-1.2.0/src/asphalt_web.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.125054 asphalt-web-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:17.129054 asphalt-web-1.2.0/tests/django_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/django_app/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_asgi3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-30 17:30:06.000000 asphalt-web-1.2.0/tests/test_starlette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.411782 asphalt-web-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.399782 asphalt-web-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.403782 asphalt-web-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-03 09:26:38.411782 asphalt-web-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.403782 asphalt-web-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/integrations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.403782 asphalt-web-1.2.1/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/modules/aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/modules/asgi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/modules/django.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/modules/fastapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/modules/starlette.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/py-modindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/docs/versionhistory.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.403782 asphalt-web-1.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.403782 asphalt-web-1.2.1/examples/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/aiohttp/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/aiohttp/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/aiohttp/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/aiohttp/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.403782 asphalt-web-1.2.1/examples/asgi3/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/asgi3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/asgi3/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/asgi3/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.403782 asphalt-web-1.2.1/examples/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/django/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/django/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.407782 asphalt-web-1.2.1/examples/django/django_example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/django/django_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/django/django_example/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/django/django_example/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/django/django_example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/django/django_example/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/django/django_example/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/django/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.407782 asphalt-web-1.2.1/examples/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/fastapi/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/fastapi/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/fastapi/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/fastapi/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.407782 asphalt-web-1.2.1/examples/starlette/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/starlette/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/starlette/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/starlette/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/examples/starlette/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:26:38.411782 asphalt-web-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.403782 asphalt-web-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.403782 asphalt-web-1.2.1/src/asphalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.407782 asphalt-web-1.2.1/src/asphalt/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/src/asphalt/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/src/asphalt/web/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/src/asphalt/web/asgi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/src/asphalt/web/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/src/asphalt/web/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/src/asphalt/web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/src/asphalt/web/starlette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.407782 asphalt-web-1.2.1/src/asphalt_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-03 09:26:38.000000 asphalt-web-1.2.1/src/asphalt_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-03 09:26:38.000000 asphalt-web-1.2.1/src/asphalt_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:26:38.000000 asphalt-web-1.2.1/src/asphalt_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 09:26:38.000000 asphalt-web-1.2.1/src/asphalt_web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-03 09:26:38.000000 asphalt-web-1.2.1/src/asphalt_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 09:26:38.000000 asphalt-web-1.2.1/src/asphalt_web.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.407782 asphalt-web-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:38.411782 asphalt-web-1.2.1/tests/django_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/django_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/django_app/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/django_app/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/django_app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/django_app/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/test_asgi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-03 09:26:25.000000 asphalt-web-1.2.1/tests/test_starlette.py
```

### Comparing `asphalt-web-1.2.0/.github/workflows/publish.yml` & `asphalt-web-1.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/.github/workflows/test.yml` & `asphalt-web-1.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/.pre-commit-config.yaml` & `asphalt-web-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/LICENSE` & `asphalt-web-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/PKG-INFO` & `asphalt-web-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asphalt-web
-Version: 1.2.0
+Version: 1.2.1
 Summary: Web framework integrations for the Asphalt framework
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Documentation, https://asphalt-web.readthedocs.org/en/latest/
 Project-URL: Source code, https://github.com/asphalt-framework/asphalt-web
 Project-URL: Issue tracker, https://github.com/asphalt-framework/asphalt-web/issues
 Project-URL: Help and support, https://github.com/asphalt-framework/asphalt/wiki/Help-and-support
```

### Comparing `asphalt-web-1.2.0/README.rst` & `asphalt-web-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/docs/conf.py` & `asphalt-web-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/docs/contributing.rst` & `asphalt-web-1.2.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/docs/integrations.rst` & `asphalt-web-1.2.1/docs/integrations.rst`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/docs/usage.rst` & `asphalt-web-1.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/examples/asgi3/static.py` & `asphalt-web-1.2.1/examples/asgi3/static.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/examples/django/django_example/settings.py` & `asphalt-web-1.2.1/examples/django/django_example/settings.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/examples/django/django_example/urls.py` & `asphalt-web-1.2.1/examples/django/django_example/urls.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/examples/django/manage.py` & `asphalt-web-1.2.1/examples/django/manage.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/pyproject.toml` & `asphalt-web-1.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -44,22 +44,25 @@
     "aiohttp >= 3.8"
 ]
 asgi3 = [
     "asgiref ~= 3.5",
     "uvicorn >= 0.17.6",
 ]
 django = [
+    "asgiref ~= 3.5",
     "Django >= 3.2",
     "uvicorn >= 0.17.6",
 ]
 fastapi = [
+    "asgiref ~= 3.5",
     "fastapi >= 0.75",
     "uvicorn >= 0.17.6",
 ]
 starlette = [
+    "asgiref ~= 3.5",
     "starlette >= 0.17",
     "uvicorn >= 0.17.6",
 ]
 test = [
     "pytest",
     "pytest-asyncio",
     "httpx",
```

### Comparing `asphalt-web-1.2.0/src/asphalt/web/aiohttp.py` & `asphalt-web-1.2.1/src/asphalt/web/aiohttp.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/src/asphalt/web/asgi3.py` & `asphalt-web-1.2.1/src/asphalt/web/asgi3.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/src/asphalt/web/django.py` & `asphalt-web-1.2.1/src/asphalt/web/django.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/src/asphalt/web/fastapi.py` & `asphalt-web-1.2.1/src/asphalt/web/fastapi.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/src/asphalt/web/starlette.py` & `asphalt-web-1.2.1/src/asphalt/web/starlette.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/src/asphalt_web.egg-info/PKG-INFO` & `asphalt-web-1.2.1/src/asphalt_web.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asphalt-web
-Version: 1.2.0
+Version: 1.2.1
 Summary: Web framework integrations for the Asphalt framework
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: Apache License 2.0
 Project-URL: Documentation, https://asphalt-web.readthedocs.org/en/latest/
 Project-URL: Source code, https://github.com/asphalt-framework/asphalt-web
 Project-URL: Issue tracker, https://github.com/asphalt-framework/asphalt-web/issues
 Project-URL: Help and support, https://github.com/asphalt-framework/asphalt/wiki/Help-and-support
```

### Comparing `asphalt-web-1.2.0/src/asphalt_web.egg-info/SOURCES.txt` & `asphalt-web-1.2.1/src/asphalt_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/tests/django_app/settings.py` & `asphalt-web-1.2.1/tests/django_app/settings.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/tests/django_app/urls.py` & `asphalt-web-1.2.1/tests/django_app/urls.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/tests/test_aiohttp.py` & `asphalt-web-1.2.1/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/tests/test_asgi3.py` & `asphalt-web-1.2.1/tests/test_asgi3.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/tests/test_django.py` & `asphalt-web-1.2.1/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/tests/test_fastapi.py` & `asphalt-web-1.2.1/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `asphalt-web-1.2.0/tests/test_starlette.py` & `asphalt-web-1.2.1/tests/test_starlette.py`

 * *Files identical despite different names*

