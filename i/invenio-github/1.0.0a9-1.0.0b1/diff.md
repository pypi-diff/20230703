# Comparing `tmp/invenio-github-1.0.0a9.tar.gz` & `tmp/invenio-github-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-github-1.0.0a9.tar", last modified: Thu Sep 29 17:41:32 2016, max compression
+gzip compressed data, was "dist/invenio-github-1.0.0b1.tar", last modified: Mon Jul  3 13:23:32 2023, max compression
```

## Comparing `invenio-github-1.0.0a9.tar` & `invenio-github-1.0.0b1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/.tx/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1795 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/.tx/config
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/docs/
--rw-rw-r--   0 travis    (1000) travis    (1000)     7441 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/Makefile
--rw-rw-r--   0 travis    (1000) travis    (1000)     1030 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/api.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/authors.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/changes.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)    10729 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/conf.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1013 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/contributing.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1571 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/index.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/installation.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)      867 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/license.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     6997 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/make.bat
--rw-rw-r--   0 travis    (1000) travis    (1000)       17 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)     1024 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/docs/usage.rst
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/examples/
--rw-rw-r--   0 travis    (1000) travis    (1000)     6592 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/examples/app.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/static/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/static/js/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/static/js/github/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1200 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/static/js/github/init.js
--rw-rw-r--   0 travis    (1000) travis    (1000)     3231 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/static/js/github/view.js
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/static/scss/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/static/scss/github/
--rw-rw-r--   0 travis    (1000) travis    (1000)     2751 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/static/scss/github/github.scss
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/templates/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/templates/invenio_github/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1249 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/base.html
--rw-rw-r--   0 travis    (1000) travis    (1000)     3702 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/helpers.html
--rw-rw-r--   0 travis    (1000) travis    (1000)     5597 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/index.html
--rw-rw-r--   0 travis    (1000) travis    (1000)     1688 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/index_item.html
--rw-rw-r--   0 travis    (1000) travis    (1000)     9012 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/view.html
--rw-rw-r--   0 travis    (1000) travis    (1000)      160 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/templates/invenio_github/base.html
--rw-rw-r--   0 travis    (1000) travis    (1000)     2078 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/templates/invenio_github/helpers.html
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/cs/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/cs/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1470 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/translations/cs/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/da/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/da/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1337 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/translations/da/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/de/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/de/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1337 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/translations/de/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/en/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/en/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      883 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/en/LC_MESSAGES/messages.mo
--rw-rw-r--   0 travis    (1000) travis    (1000)     1776 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/translations/en/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/es/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/es/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1338 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/translations/es/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/fr/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/fr/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1551 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/translations/fr/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/it/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/translations/it/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1556 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/translations/it/LC_MESSAGES/messages.po
--rw-rw-r--   0 travis    (1000) travis    (1000)     1271 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/translations/messages.pot
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github/views/
--rw-rw-r--   0 travis    (1000) travis    (1000)      989 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/views/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2877 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/views/badge.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7848 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/views/github.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1222 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2378 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/admin.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    15839 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/api.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1715 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/bundles.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3220 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/config.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1515 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/errors.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3484 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/ext.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4018 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/handlers.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    11457 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/models.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1216 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/proxies.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2946 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/receivers.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5263 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/tasks.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3435 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/utils.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1183 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/invenio_github/version.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)     4708 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)     2439 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      750 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-09-29 17:40:53.000000 invenio-github-1.0.0a9/invenio_github.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (1000) travis    (1000)     1016 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github.egg-info/requires.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       21 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/invenio_github.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/tests/
--rw-rw-r--   0 travis    (1000) travis    (1000)        0 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/tests/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    12517 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/tests/conftest.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    25908 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/tests/fixtures.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2252 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/tests/helpers.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1604 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/tests/test_badge.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1601 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/tests/test_invenio_github.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1202 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/tests/test_models.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3310 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/tests/test_tasks.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1948 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/tests/test_webhook.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      124 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/.dockerignore
--rw-rw-r--   0 travis    (1000) travis    (1000)     1533 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/.editorconfig
--rw-rw-r--   0 travis    (1000) travis    (1000)     1278 2016-09-29 17:40:33.000000 invenio-github-1.0.0a9/.travis-devel-requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      436 2016-09-29 17:40:33.000000 invenio-github-1.0.0a9/.travis-lowest-requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      455 2016-09-29 17:40:33.000000 invenio-github-1.0.0a9/.travis-release-requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)     1349 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/AUTHORS.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1063 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/CHANGES.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     3466 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)       26 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/INSTALL.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)    18092 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/LICENSE
--rw-rw-r--   0 travis    (1000) travis    (1000)     1594 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/MANIFEST.in
--rw-rw-r--   0 travis    (1000) travis    (1000)     1984 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/README.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)      759 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/RELEASE-NOTES.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1289 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/babel.ini
--rw-rw-r--   0 travis    (1000) travis    (1000)     1059 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/pytest.ini
--rw-rw-r--   0 travis    (1000) travis    (1000)     1902 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/requirements-devel.txt
--rwxrwxr-x   0 travis    (1000) travis    (1000)     1220 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/run-tests.sh
--rw-rw-r--   0 travis    (1000) travis    (1000)      662 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/setup.cfg
--rw-rw-r--   0 travis    (1000) travis    (1000)     4921 2016-09-29 17:40:17.000000 invenio-github-1.0.0a9/setup.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4708 2016-09-29 17:41:32.000000 invenio-github-1.0.0a9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.lgtm
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1134 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4311 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/RELEASE-NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10752 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21716 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/invenio_github/init.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3733 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/invenio_github/view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/less/github/
+-rw-r--r--   0 runner    (1001) docker     (122)     3013 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/less/github/github.scss
+-rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3498 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8658 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4777 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/helpers.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3702 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5597 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
+-rw-r--r--   0 runner    (1001) docker     (122)    10522 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/views/badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/views/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/invenio_github/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4311 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2500 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/invenio_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 13:23:32.000000 invenio-github-1.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8804 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21853 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_invenio_github.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3608 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3713 2023-07-03 13:23:23.000000 invenio-github-1.0.0b1/tests/test_webhook.py
```

### Comparing `invenio-github-1.0.0a9/.tx/config` & `invenio-github-1.0.0b1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/Makefile` & `invenio-github-1.0.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/api.rst` & `invenio-github-1.0.0b1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/authors.rst` & `invenio-github-1.0.0b1/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/changes.rst` & `invenio-github-1.0.0b1/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/conf.py` & `invenio-github-1.0.0b1/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2016 CERN.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -18,317 +19,316 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
-from __future__ import print_function
+"""Sphinx configuration."""
 
-import os
-
-import sphinx.environment
+from invenio_github import __version__
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Do not warn on external images.
-suppress_warnings = ['image.nonlocal_uri']
+suppress_warnings = ["image.nonlocal_uri"]
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.coverage',
-    'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'Invenio-GitHub'
-copyright = u'2016, CERN'
-author = u'CERN'
+project = "Invenio-GitHub"
+copyright = "2016, CERN"
+author = "CERN"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 
-# Get the version string. Cannot be done with import!
-g = {}
-with open(os.path.join('..', 'invenio_github', 'version.py'), 'rt') as fp:
-    exec(fp.read(), g)
-    version = g['__version__']
-
 # The full version, including alpha/beta/rc tags.
-release = version
+release = __version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 html_theme_options = {
-    'description': 'Invenio module that adds GitHub integration to the platform.',
-    'github_user': 'inveniosoftware',
-    'github_repo': 'invenio-github',
-    'github_button': False,
-    'github_banner': True,
-    'show_powered_by': False,
-    'extra_nav_links': {
-        'invenio-github@GitHub': 'https://github.com/inveniosoftware/invenio-github',
-        'invenio-github@PyPI': 'https://pypi.python.org/pypi/invenio-github/',
-    }
+    "description": "Invenio module that adds GitHub integration to the platform.",
+    "github_user": "inveniosoftware",
+    "github_repo": "invenio-github",
+    "github_button": False,
+    "github_banner": True,
+    "show_powered_by": False,
+    "extra_nav_links": {
+        "invenio-github@GitHub": "https://github.com/inveniosoftware/invenio-github",
+        "invenio-github@PyPI": "https://pypi.python.org/pypi/invenio-github/",
+    },
 }
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-#html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
 html_sidebars = {
-    '**': [
-        'about.html',
-        'navigation.html',
-        'relations.html',
-        'searchbox.html',
-        'donate.html',
+    "**": [
+        "about.html",
+        "navigation.html",
+        "relations.html",
+        "searchbox.html",
+        "donate.html",
     ]
 }
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Language to be used for generating the HTML full-text search index.
 # Sphinx supports the following languages:
 #   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
 #   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
-#html_search_language = 'en'
+# html_search_language = 'en'
 
 # A dictionary with options for the search language support, empty by default.
 # Now only 'ja' uses this config value
-#html_search_options = {'type': 'default'}
+# html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
+# html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'invenio-github_namedoc'
+htmlhelp_basename = "invenio-github_namedoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-
-# Latex figure (float) alignment
-#'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
+    # Latex figure (float) alignment
+    #'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  (master_doc, 'invenio-github.tex', u'invenio-github Documentation',
-   u'CERN', 'manual'),
+    (
+        master_doc,
+        "invenio-github.tex",
+        "invenio-github Documentation",
+        "CERN",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'invenio-github', u'invenio-github Documentation',
-     [author], 1)
+    (master_doc, "invenio-github", "invenio-github Documentation", [author], 1)
 ]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  (master_doc, 'invenio-github', u'Invenio-GitHub Documentation',
-   author, 'invenio-github', 'Invenio module that adds GitHub integration to the platform.',
-   'Miscellaneous'),
+    (
+        master_doc,
+        "invenio-github",
+        "Invenio-GitHub Documentation",
+        author,
+        "invenio-github",
+        "Invenio module that adds GitHub integration to the platform.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {"https://docs.python.org/": None}
 
 # Autodoc configuraton.
-autoclass_content = 'both'
+autoclass_content = "both"
```

### Comparing `invenio-github-1.0.0a9/docs/contributing.rst` & `invenio-github-1.0.0b1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/index.rst` & `invenio-github-1.0.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/installation.rst` & `invenio-github-1.0.0b1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/license.rst` & `invenio-github-1.0.0b1/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/make.bat` & `invenio-github-1.0.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/docs/usage.rst` & `invenio-github-1.0.0b1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/static/js/github/init.js` & `invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/invenio_github/init.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -16,18 +16,18 @@
  * along with Invenio. If not, see <http://www.gnu.org/licenses/>.
  *
  * In applying this licence, CERN does not waive the privileges and immunities
  * granted to it by virtue of its status as an Intergovernmental Organization
  * or submit itself to any jurisdiction.
  */
 
-require([
-    'jquery',
-    'node_modules/bootstrap-switch/dist/js/bootstrap-switch',
-    'js/github/view'
-], function() {
-    /*
-     * It preloads js/github/view to give it a name so you're free to use it
-     * from any places.
-     */
-    console.info("js/github/init is loaded");
-});
+// require([
+//   'jquery',
+//   'node_modules/bootstrap-switch/dist/js/bootstrap-switch',
+//   'js/github/view'
+//   ], function() {
+//     /*
+//      * It preloads js/github/view to give it a name so you're free to use it
+//      * from any places.
+//      */
+//     console.info("js/github/init is loaded");
+// });
```

### Comparing `invenio-github-1.0.0a9/invenio_github/static/js/github/view.js` & `invenio-github-1.0.0b1/invenio_github/assets/semantic-ui/js/invenio_github/view.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,108 +1,109 @@
-/*
- * This file is part of Invenio.
- * Copyright (C) 2014, 2015, 2016 CERN.
- *
- * Invenio is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, either version 3 of the License, or
- * (at your option) any later version.
- *
- * Invenio is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with Invenio. If not, see <http://www.gnu.org/licenses/>.
- *
- * In applying this licence, CERN does not waive the privileges and immunities
- * granted to it by virtue of its status as an Intergovernmental Organization
- * or submit itself to any jurisdiction.
- */
-define(function(require, exports, module) {
-    'use strict';
-
-    var $ = require('jquery');
-    require('node_modules/bootstrap-switch/dist/js/bootstrap-switch');
-
-    return function(config) {
-        init_switches(config);
-        init_syncbutton(config);
-
-        $('[data-toggle="tooltip"]').tooltip();
-
-        $('i.error').tooltip({
-            trigger: 'hover',
-            animation: true,
-            placement: 'top',
-        });
-    };
-
-    function init_syncbutton(config) {
-        var syncButton = $(config.sync_button);
-
-        syncButton.on('click', function() {
-            syncButton.prop('disabled', true);
-            $.ajax({
-                    url: config.sync_url,
-                    type: 'POST'
-                })
-                .done(function(data) {
-                    $(config.github_view).html(data);
-                    init_switches(config);
-                    init_syncbutton(config);
-                })
-                .always(function() {
-                    syncButton.prop('disabled', false);
-                });
-        });
-    }
-
-    function init_switches(config) {
-        // Initialize bootstrap switches
-        var test_switch = $('input[name="test-flip"]').bootstrapSwitch();
-        var doiSwitches = $('input[data-repo-id]').bootstrapSwitch();
-
-        doiSwitches.on('switchChange.bootstrapSwitch', function(e, state) {
-            // Disable the switch
-            var $switch = $(e.target);
-            $switch.bootstrapSwitch('disabled', true);
-            var repoId = e.target.dataset.repoId;
-            var method = state ? 'POST' : 'DELETE';
-
-            $.ajax({
-                    url: config.hook_url,
-                    type: method,
-                    data: JSON.stringify({
-                        id: repoId
-                    }),
-                    contentType: 'application/json; charset=utf-8',
-                    dataType: 'json'
-                })
-                .done(function(data, textStatus, jqXHR) {
-                    var status = 'fa-exclamation text-warning';
-                    if (jqXHR.status == 204 || jqXHR.status == 201) {
-                        status = 'fa-check text-success';
-                    }
-
-                    // Select the correct hook status
-                    var el = $('[data-repo-id="' + repoId + '"].hook-status');
-                    el.addClass(status);
-                    el.animate({
-                        opacity: 0
-                    }, 2000, function() {
-                        el.removeClass(status);
-                        el.css('opacity', 1);
-                    });
-                })
-                .fail(function() {
-                    // Revert back to normal
-                    $switch.bootstrapSwitch('state', !state);
-                })
-                .always(function() {
-                    // Enable the switch
-                    $switch.bootstrapSwitch('disabled', false);
-                });
-        });
-    }
-});
+// /*
+//  * This file is part of Invenio.
+//  * Copyright (C) 2014, 2015, 2016 CERN.
+//  *
+//  * Invenio is free software: you can redistribute it and/or modify
+//  * it under the terms of the GNU General Public License as published by
+//  * the Free Software Foundation, either version 3 of the License, or
+//  * (at your option) any later version.
+//  *
+//  * Invenio is distributed in the hope that it will be useful,
+//  * but WITHOUT ANY WARRANTY; without even the implied warranty of
+//  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+//  * GNU General Public License for more details.
+//  *
+//  * You should have received a copy of the GNU General Public License
+//  * along with Invenio. If not, see <http://www.gnu.org/licenses/>.
+//  *
+//  * In applying this licence, CERN does not waive the privileges and immunities
+//  * granted to it by virtue of its status as an Intergovernmental Organization
+//  * or submit itself to any jurisdiction.
+//  */
+// define(function (require, exports, module) {
+//   'use strict';
+
+//   var $ = require('jquery');
+//   require('node_modules/bootstrap-switch/dist/js/bootstrap-switch');
+
+//   return function (config) {
+//     init_switches(config);
+//     init_syncbutton(config);
+
+//     $('[data-toggle="tooltip"]').tooltip();
+
+//     $('i.error').tooltip({
+//       trigger: 'hover',
+//       animation: true,
+//       placement: 'top',
+//     });
+//   };
+
+//   function init_syncbutton(config) {
+//     var syncButton = $(config.sync_button);
+//     var syncIcon = $(syncButton.children()[0])
+
+//     syncButton.on('click', function () {
+//       syncButton.prop('disabled', true);
+//       syncIcon.addClass('fa-spin');
+//       $.ajax({
+//         url: config.sync_url,
+//         type: 'POST'
+//       })
+//         .done(function (data) {
+//           $(config.github_view).html(data);
+//           init_switches(config);
+//           init_syncbutton(config);
+//         })
+//         .always(function () {
+//           syncButton.prop('disabled', false);
+//           syncIcon.removeClass('fa-spin');
+//         });
+//     });
+//   }
+
+//   function init_switches(config) {
+//     // Initialize bootstrap switches
+//     var test_switch = $('input[name="test-flip"]').bootstrapSwitch();
+//     var doiSwitches = $('input[data-repo-id]').bootstrapSwitch();
+
+//     doiSwitches.on('switchChange.bootstrapSwitch', function (e, state) {
+//       // Disable the switch
+//       var $switch = $(e.target);
+//       $switch.bootstrapSwitch('disabled', true);
+//       var repoId = e.target.dataset.repoId;
+//       var method = state ? 'POST' : 'DELETE';
+
+//       $.ajax({
+//         url: config.hook_url,
+//         type: method,
+//         data: JSON.stringify({ id: repoId }),
+//         contentType: 'application/json; charset=utf-8',
+//         dataType: 'json'
+//       })
+//         .done(function (data, textStatus, jqXHR) {
+//           var status = 'fa-exclamation text-warning';
+//           if (jqXHR.status == 204 || jqXHR.status == 201) {
+//             status = 'fa-check text-success';
+//           }
+
+//           // Select the correct hook status
+//           var el = $('[data-repo-id="' + repoId + '"].hook-status');
+//           el.addClass(status);
+//           el.animate({
+//             opacity: 0
+//           }, 2000, function () {
+//             el.removeClass(status);
+//             el.css('opacity', 1);
+//           });
+//         })
+//         .fail(function () {
+//           // Revert back to normal
+//           $switch.bootstrapSwitch('state', !state);
+//         })
+//         .always(function () {
+//           // Enable the switch
+//           $switch.bootstrapSwitch('disabled', false);
+//         });
+//     });
+//   }
+// });
```

### Comparing `invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/base.html` & `invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/base.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/helpers.html` & `invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/index.html` & `invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/index_item.html` & `invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/templates/invenio_github/settings/view.html` & `invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/settings/view.html`

 * *Files 18% similar despite different names*

```diff
@@ -123,74 +123,99 @@
                 <a href="https://doi.org/{{release.pid.pid_value}}" class="text-muted">
                   <i class="fa fa-fw fa-barcode"></i>
                   DOI: {{release.pid.pid_value}}
                 </a>
               </p>
               {%- endif %}
               <p>
-                <a href="{{release.event.payload.release.html_url if release.event else 'https://github.com/{0}/releases/tag/{1}'.format(repo.name, release.model.tag)}}" class="text-muted">
+                <a href="{{ release.event.payload.release.html_url if release.event else 'https://github.com/{0}/releases/tag/{1}'.format(repo.name, release.model.tag)}}" class="text-muted">
                   <i class="fa fa-fw fa-github"></i>
                   {{release.event.payload.release.name if release.event and release.event.payload.release.name else release.model.tag}}
                 </a>
               </p>
               {%- endblock release_title %}
           </div>
           <div class="col-md-3">
             {%- block release_status scoped %}
             <h5>
               <i class="fa {{ release.model.status.icon }}"></i>
               <a href="#" data-toggle="collapse" data-target="#{{ release.model.id }}">
-              {{_(release.model.status.title)}}
+              {{release.model.status.title}}
               </a>
             </h5>
             <small class="text-muted">{{ release.model.created|naturaltime }}</small>
             {%- endblock release_status %}
           </div>
         </div>
       </div>
       {%- endblock release_header %}
       {%- block release_body scoped %}
       <div id="{{ release.model.id }}" class="panel-body release {{release.model.status.title|lower}} collapse">
         <ul class="nav nav-tabs" role="tablist">
-          {%- if release.event %}
           <li class="active">
+            <a href="#{{ release.model.id }}-cff" data-toggle="tab">{{ _('Citation File') }}</a>
+          </li>
+          {%- if release.event %}
+          <li>
             <a href="#{{ release.model.id }}-event" data-toggle="tab">{{ _('Payload') }}</a>
           </li>
           {%- endif %}
-          {%- if release.record %}
+          {%- if release.status == 'D' %}
           <li>
             <a href="#{{ release.model.id }}-metadata" data-toggle="tab">{{ _('Metadata') }}</a>
           </li>
           {%- endif %}
           {%- if release.model.errors %}
           <li>
             <a href="#{{ release.model.id }}-errors" data-toggle="tab">{{ _('Errors') }}</a>
           </li>
           {%- endif %}
         </ul>
         <div class="tab-content">
+          {%- block releasetab_cff scoped %}
+          {% set repo_name = value %}
+          {% set citation_cff_create_link = 'https://github.com/{0}/new/{1}?filename=CITATION.cff'.format(repo.name, (repo_info.default_branch or 'master')) %}
+          <div role="tabpanel" class="tab-pane active" id="{{ release.model.id }}-cff">
+            <a target="_blank" class="pull-right btn btn-xs btn-default" href="{{ citation_cff_create_link }}"><i class="fa fa-github"></i> Create CITATION.cff</a>
+            <h4>Citation File</h4>
+            <p><a href="https://citation-file-format.github.io/">CITATION.cff</a> files are plain text files with human- and machine-readable citation information for software. Code developers can include them in their repositories to let others know how to correctly cite their software.</p>
+            <p>An example of the CITATION.cff for this release can be found below:</p>
+            <pre>
+cff-version: 1.1.0
+message: "If you use this software, please cite it as below."
+authors:
+  - family-names: Joe
+    given-names: Johnson
+    orcid: https://orcid.org/0000-0000-0000-0000
+title: {{ release.title }}
+version: {{ release.model.tag }}
+date-released: {{ release.event.payload.release.published_at[:10] if release.event else '2021-07-28' }}
+            </pre>
+          </div>
+          {%- endblock releasetab_cff %}
           {%- if release.event %}
           {%- block releasetab_payload scoped %}
-          <div role="tabpanel" class="tab-pane active" id="{{ release.model.id }}-event">
+          <div role="tabpanel" class="tab-pane" id="{{ release.model.id }}-event">
             <small class="text-muted pull-right">{{_('Received')}} {{release.event.created|datetimeformat}}.</small>
             <h4>GitHub Payload</h4>
             <pre>{{ release.event.payload|tojson|prettyjson }}</pre>
           </div>
           {%- endblock releasetab_payload %}
           {%- endif %}
-          {%- if release.record %}
+          {%- if release.status == 'D' %}
           {%- block releasetab_metadata scoped %}
           <div role="tabpanel" class="tab-pane" id="{{ release.model.id }}-metadata">
             <h4>{{_('JSON Export')}}</h4>
             <p>
             <small class="text-muted">
               {{config.THEME_SITENAME | default('Invenio')}} automatically
-              extracts metadata about your repository from GitHub APIs. The
-              authors are e.g. determined from the repository's contributor
-              statistics. The automatic extraction is <strong>solely a best
+              extracts metadata about your repository from GitHub APIs.
+              For example, the authors are determined from the
+              repository's contributor statistics.
+              The automatic extraction is <strong>solely a best
               guess</strong>. Add a
               <code>{{config.GITHUB_METADATA_FILE}}</code> file the root of
               your repository to explicit define the metadata. The format of
               file is the same as for our REST API (use e.g. below JSON to
               get started).
             </small>
             </p>
```

### Comparing `invenio-github-1.0.0a9/invenio_github/templates/invenio_github/helpers.html` & `invenio-github-1.0.0b1/invenio_github/templates/semantic-ui/invenio_github/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/translations/cs/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b1/invenio_github/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/translations/da/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b1/invenio_github/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/translations/de/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b1/invenio_github/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/translations/en/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b1/invenio_github/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/translations/es/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b1/invenio_github/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/translations/fr/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b1/invenio_github/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/translations/it/LC_MESSAGES/messages.po` & `invenio-github-1.0.0b1/invenio_github/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/translations/messages.pot` & `invenio-github-1.0.0b1/invenio_github/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/invenio_github/views/__init__.py` & `invenio-github-1.0.0b1/invenio_github/views/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,9 +17,7 @@
 # along with Invenio. If not, see <http://www.gnu.org/licenses/>.
 #
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
 
 """Implement views for GitHub integration."""
-
-from __future__ import absolute_import
```

### Comparing `invenio-github-1.0.0a9/invenio_github/views/badge.py` & `invenio-github-1.0.0b1/invenio_github/views/badge.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,64 +27,68 @@
 
 from flask import Blueprint, abort, redirect, url_for
 
 from ..api import GitHubRelease
 from ..models import ReleaseStatus, Repository
 
 blueprint = Blueprint(
-    'invenio_github_badge',
+    "invenio_github_badge",
     __name__,
-    url_prefix='/badge',
-    static_folder='../static',
-    template_folder='../templates',
+    url_prefix="/badge",
+    static_folder="../static",
+    template_folder="../templates",
 )
 
 
 def get_pid_of_latest_release_or_404(**kwargs):
     """Return PID of the latest release."""
     repo = Repository.query.filter_by(**kwargs).first_or_404()
     release = repo.latest_release(ReleaseStatus.PUBLISHED)
     if release:
         return GitHubRelease(release).pid
     abort(404)
 
 
-def get_badge_image_url(pid, ext='svg'):
+def get_badge_image_url(pid, ext="svg"):
     """Return the badge for a DOI."""
-    return url_for('invenio_formatter_badges.badge',
-                   title=pid.pid_type, value=pid.pid_value, ext=ext)
+    return url_for(
+        "invenio_formatter_badges.badge",
+        title=pid.pid_type,
+        value=pid.pid_value,
+        ext=ext,
+    )
 
 
 def get_doi_url(pid):
     """Return the badge for a DOI."""
-    return 'https://doi.org/{pid.pid_value}'.format(pid=pid)
+    return "https://doi.org/{pid.pid_value}".format(pid=pid)
 
 
 #
 # Views
 #
-@blueprint.route('/<int:github_id>.svg')
+@blueprint.route("/<int:github_id>.svg")
 def index(github_id):
     """Generate a badge for a specific GitHub repository."""
     pid = get_pid_of_latest_release_or_404(github_id=github_id)
     return redirect(get_badge_image_url(pid))
 
 
-@blueprint.route('/<int:user_id>/<path:repo_name>.svg')
+@blueprint.route("/<int:user_id>/<path:repo_name>.svg")
 def index_old(user_id, repo_name):
     """Generate a badge for a specific GitHub repository."""
     pid = get_pid_of_latest_release_or_404(name=repo_name)
     return redirect(get_badge_image_url(pid))
 
 
-@blueprint.route('/latestdoi/<int:github_id>')
+@blueprint.route("/latestdoi/<int:github_id>")
 def latest_doi(github_id):
     """Redirect to the newest record version."""
     pid = get_pid_of_latest_release_or_404(github_id=github_id)
     return redirect(get_doi_url(pid))
 
 
-@blueprint.route('/latestdoi/<int:user_id>/<path:repo_name>')
+@blueprint.route("/latestdoi/<int:user_id>/<path:repo_name>")
 def latest_doi_old(user_id, repo_name):
     """Redirect to the newest record version."""
     pid = get_pid_of_latest_release_or_404(name=repo_name)
     return redirect(get_doi_url(pid))
```

### Comparing `invenio-github-1.0.0a9/invenio_github/views/github.py` & `invenio-github-1.0.0b1/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,247 +1,293 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2014, 2015, 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
-# Invenio is free software; you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Invenio is free software; you can redistribute it
+# and/or modify it under the terms of the GNU General Public License as
+# published by the Free Software Foundation; either version 2 of the
+# License, or (at your option) any later version.
 #
-# Invenio is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# Invenio is distributed in the hope that it will be
+# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with Invenio. If not, see <http://www.gnu.org/licenses/>.
+# along with Invenio; if not, write to the
+# Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
+# MA 02111-1307, USA.
 #
-# In applying this licence, CERN does not waive the privileges and immunities
-# granted to it by virtue of its status as an Intergovernmental Organization
-# or submit itself to any jurisdiction.
-
-"""GitHub blueprint for Invenio platform."""
-
-from __future__ import absolute_import
-
-import json
-from datetime import datetime
-
-import humanize
-import pytz
-from dateutil.parser import parse
-from flask import Blueprint, abort, current_app, redirect, render_template, \
-    request, url_for
-from flask_babelex import gettext as _
-from flask_breadcrumbs import register_breadcrumb
-from flask_login import current_user, login_required
-from flask_menu import register_menu
-from invenio_db import db
-from sqlalchemy.orm.exc import NoResultFound
-
-from ..api import GitHubAPI, GitHubRelease
-from ..errors import RepositoryAccessError
-from ..models import Release, Repository
-from ..proxies import current_github
-from ..utils import parse_timestamp, utcnow
-
-blueprint = Blueprint(
-    'invenio_github',
-    __name__,
-    static_folder='../static',
-    template_folder='../templates',
-    url_prefix='/account/settings/github',
+# In applying this license, CERN does not
+# waive the privileges and immunities granted to it by virtue of its status
+# as an Intergovernmental Organization or submit itself to any jurisdiction.
+
+"""Pytest configuration."""
+
+from __future__ import absolute_import, print_function
+
+from collections import namedtuple
+
+import pytest
+from invenio_app.factory import create_api
+from invenio_oauthclient.contrib.github import REMOTE_APP as GITHUB_REMOTE_APP
+from invenio_oauthclient.contrib.github import REMOTE_REST_APP as GITHUB_REMOTE_REST_APP
+from invenio_oauthclient.models import RemoteToken
+from invenio_oauthclient.proxies import current_oauthclient
+from mock import MagicMock, patch
+
+from .fixtures import (
+    TestGithubRelease,
+    github_file_contents,
+    github_repo_metadata,
+    github_user_metadata,
 )
 
 
-#
-# Template filters
-#
-@blueprint.app_template_filter('naturaltime')
-def naturaltime(val):
-    """Get humanized version of time."""
-    val = val.replace(tzinfo=pytz.utc) \
-        if isinstance(val, datetime) else parse(val)
-    now = datetime.utcnow().replace(tzinfo=pytz.utc)
-
-    return humanize.naturaltime(now - val)
-
-
-@blueprint.app_template_filter('prettyjson')
-def prettyjson(val):
-    """Get pretty-printed json."""
-    return json.dumps(json.loads(val), indent=4)
-
-
-@blueprint.app_template_filter('release_pid')
-def release_pid(release):
-    """Get PID of Release record."""
-    return GitHubRelease(release).pid
+@pytest.fixture(scope="module")
+def app_config(app_config):
+    """Test app config."""
+    app_config.update(
+        # HTTPretty doesn't play well with Redis.
+        # See gabrielfalcao/HTTPretty#110
+        APP_THEME=[],
+        CACHE_TYPE="simple",
+        CELERY_ALWAYS_EAGER=True,
+        CELERY_CACHE_BACKEND="memory",
+        CELERY_EAGER_PROPAGATES_EXCEPTIONS=True,
+        CELERY_RESULT_BACKEND="cache",
+        GITHUB_APP_CREDENTIALS=dict(
+            consumer_key="changeme",
+            consumer_secret="changeme",
+        ),
+        GITHUB_SHARED_SECRET="changeme",
+        GITHUB_INSECURE_SSL=False,
+        GITHUB_METADATA_FILE=".invenio.json",
+        GITHUB_WEBHOOK_RECEIVER_URL="http://localhost:5000/api/receivers/github/events/?access_token={token}",
+        GITHUB_WEBHOOK_RECEIVER_ID="github",
+        GITHUB_RELEASE_CLASS=TestGithubRelease,
+        LOGIN_DISABLED=False,
+        OAUTHLIB_INSECURE_TRANSPORT=True,
+        OAUTH2_CACHE_TYPE="simple",
+        OAUTHCLIENT_REMOTE_APPS=dict(
+            github=GITHUB_REMOTE_APP,
+        ),
+        OAUTHCLIENT_REST_REMOTE_APPS=dict(
+            github=GITHUB_REMOTE_REST_APP,
+        ),
+        SECRET_KEY="test_key",
+        SERVER_NAME="testserver",
+        SECURITY_PASSWORD_HASH="plaintext",
+        SECURITY_PASSWORD_SCHEMES=["plaintext"],
+        SECURITY_DEPRECATED_PASSWORD_SCHEMES=[],
+        TESTING=True,
+        WTF_CSRF_ENABLED=False,
+        JSONSCHEMAS_HOST="not-used",
+        RECORDS_REFRESOLVER_CLS="invenio_records.resolver.InvenioRefResolver",
+        RECORDS_REFRESOLVER_STORE="invenio_jsonschemas.proxies.current_refresolver_store",
+        # Storage classes
+        FILES_REST_STORAGE_CLASS_LIST=dict(
+            L="Local",
+            F="Fetch",
+            R="Remote",
+        ),
+        FILES_REST_DEFAULT_STORAGE_CLASS="L",
+    )
+    app_config["OAUTHCLIENT_REMOTE_APPS"]["github"]["params"]["request_token_params"][
+        "scope"
+    ] = "user:email,admin:repo_hook,read:org"
+    return app_config
+
+
+@pytest.fixture(scope="module")
+def create_app(instance_path):
+    """Application factory fixture."""
+    return create_api
+
+
+RunningApp = namedtuple(
+    "RunningApp",
+    [
+        "app",
+        "location",
+        "cache",
+    ],
+)
 
 
-#
-# Views
-#
-@blueprint.route('/', methods=['GET', 'POST'])
-@login_required
-@register_menu(
-    blueprint, 'settings.github',
-    '<i class="fa fa-github fa-fw"></i> GitHub',
-    order=10,
-    active_when=lambda: request.endpoint.startswith('invenio_github.')
-)
-@register_breadcrumb(blueprint, 'breadcrumbs.settings.github', _('GitHub'))
-def index():
-    """Display list of the user's repositories."""
-    github = GitHubAPI(user_id=current_user.id)
-    token = github.session_token
-    ctx = dict(connected=False)
-
-    if token:
-        # The user is authenticated and the token we have is still valid.
-        if github.account.extra_data.get('login') is None:
-            github.init_account()
-            db.session.commit()
-
-        # Sync if needed
-        if request.method == 'POST' or github.check_sync():
-            # When we're in an XHR request, we want to synchronously sync hooks
-            github.sync(async_hooks=(not request.is_xhr))
-            db.session.commit()
-
-        # Generate the repositories view object
-        extra_data = github.account.extra_data
-        repos = extra_data['repos']
-        if repos:
-            # 'Enhance' our repos dict, from our database model
-            db_repos = Repository.query.filter(
-                Repository.github_id.in_([int(k) for k in repos.keys()]),
-            ).all()
-            for repo in db_repos:
-                repos[str(repo.github_id)]['instance'] = repo
-                repos[str(repo.github_id)]['latest'] = GitHubRelease(
-                    repo.latest_release())
-
-        last_sync = humanize.naturaltime(
-            (utcnow() - parse_timestamp(extra_data['last_sync'])))
-
-        ctx.update({
-            'connected': True,
-            'repos': sorted(repos.items(), key=lambda x: x[1]['full_name']),
-            'last_sync': last_sync,
-        })
-
-    return render_template(current_app.config['GITHUB_TEMPLATE_INDEX'], **ctx)
-
-
-@blueprint.route('/repository/<path:name>')
-@login_required
-@register_breadcrumb(blueprint, 'breadcrumbs.settings.github.repo',
-                     _('Repository'))
-def repository(name):
-    """Display selected repository."""
-    user_id = current_user.id
-    github = GitHubAPI(user_id=user_id)
-    token = github.session_token
-
-    if token:
-        repos = github.account.extra_data.get('repos', [])
-        repo = next((repo for repo_id, repo in repos.items()
-                     if repo.get('full_name') == name), {})
-        if not repo:
-            abort(403)
-
-        try:
-            # NOTE: Here we do not check for repository ownership, since it
-            # might have changed even though the user might have made releases
-            # in the past.
-            repo_instance = Repository.get(user_id=user_id,
-                                           github_id=repo['id'],
-                                           check_owner=False)
-        except RepositoryAccessError:
-            abort(403)
-        except NoResultFound:
-            repo_instance = Repository(name=repo['full_name'],
-                                       github_id=repo['id'])
-
-        releases = [
-            current_github.release_api_class(r) for r in (
-                repo_instance.releases.order_by(db.desc(Release.created)).all()
-                if repo_instance.id else []
-            )
-        ]
-        return render_template(
-            current_app.config['GITHUB_TEMPLATE_VIEW'],
-            repo=repo_instance,
-            releases=releases,
-            serializer=current_github.record_serializer,
+@pytest.fixture()
+def running_app(app, location, cache):
+    """This fixture provides an app with the typically needed db data loaded.
+
+    All of these fixtures are often needed together, so collecting them
+    under a semantic umbrella makes sense.
+    """
+    return RunningApp(app, location, cache)
+
+
+@pytest.fixture()
+def test_user(app, db, github_remote_app):
+    """Creates a test user.
+
+    Links the user to a github RemoteToken.
+    """
+    datastore = app.extensions["security"].datastore
+    user = datastore.create_user(
+        email="info@inveniosoftware.org",
+        password="tester",
+    )
+
+    # Create GitHub link for user
+    token = RemoteToken.get(user.id, github_remote_app.consumer_key)
+    if not token:
+        RemoteToken.create(
+            user.id,
+            github_remote_app.consumer_key,
+            "test",
+            "",
         )
-
-    abort(403)
+    db.session.commit()
+    return user
 
 
-@blueprint.route('/rejected')
-@login_required
-def rejected():
-    """View for when user rejects request to connect to github."""
-    return render_template('invenio_github/settings/rejected.html')
-
-
-@blueprint.route('/hook', methods=['POST', 'DELETE'])
-@login_required
-def hook():
-    """Install or remove GitHub webhook."""
-    repo_id = request.json['id']
-
-    github = GitHubAPI(user_id=current_user.id)
-    repos = github.account.extra_data['repos']
-
-    if repo_id not in repos:
-        abort(404)
-
-    if request.method == 'DELETE':
-        try:
-            if github.remove_hook(repo_id, repos[repo_id]['full_name']):
-                db.session.commit()
-                return '', 204
-            else:
-                abort(400)
-        except Exception:
-            abort(403)
-    elif request.method == 'POST':
-        try:
-            if github.create_hook(repo_id, repos[repo_id]['full_name']):
-                db.session.commit()
-                return '', 201
-            else:
-                abort(400)
-        except Exception:
-            abort(403)
-    else:
-        abort(400)
-
-
-@blueprint.route('/hook/<action>/<repo_id>')
-@login_required
-def hook_action(action, repo_id):
-    """Display selected repository."""
-    github = GitHubAPI(user_id=current_user.id)
-    repos = github.account.extra_data['repos']
-
-    if repo_id not in repos:
-        abort(404)
-
-    if action == 'disable':
-        if github.remove_hook(repo_id, repos[repo_id]['full_name']):
-            db.session.commit()
-            return redirect(url_for('.index'))
-        else:
-            abort(400)
-    elif action == 'enable':
-        if github.create_hook(repo_id, repos[repo_id]['full_name']):
-            db.session.commit()
-            return redirect(url_for('.index'))
-        else:
-            abort(400)
-    else:
-        abort(400)
+@pytest.fixture()
+def github_remote_app():
+    """Returns github remote app."""
+    return current_oauthclient.oauth.remote_apps["github"]
+
+
+@pytest.fixture()
+def remote_token(test_user, github_remote_app):
+    """Returns github RemoteToken for user."""
+    token = RemoteToken.get(
+        test_user.id,
+        github_remote_app.consumer_key,
+    )
+    return token
+
+
+@pytest.fixture
+def unlinked_user(app, db):
+    """Creates an user that is not linked to a remote account."""
+    datastore = app.extensions["security"].datastore
+    user = datastore.create_user(
+        email="unlinked@inveniosoftware.org",
+        password="unlinked",
+    )
+    db.session.commit()
+    return user
+
+
+@pytest.fixture()
+def tester_id(test_user):
+    """Returns tester id."""
+    return test_user.id
+
+
+@pytest.fixture()
+def test_repo_data_one():
+    """Test repository."""
+    return {"name": "repo-1", "id": 1}
+
+
+@pytest.fixture()
+def test_repo_data_two():
+    """Test repository."""
+    return {"name": "repo-2", "id": 2}
+
+
+@pytest.fixture()
+def test_repo_data_three():
+    """Test repository."""
+    return {"name": "arepo", "id": 3}
+
+
+@pytest.yield_fixture()
+def github_api(
+    running_app, db, test_repo_data_one, test_repo_data_two, test_repo_data_three
+):
+    """Github API mock."""
+    import github3
+
+    from . import fixtures
+
+    mock_api = MagicMock()
+    mock_api.session = MagicMock()
+    mock_api.me.return_value = github3.users.User(
+        github_user_metadata(login="auser", email="auser@inveniosoftware.org"),
+        mock_api.session,
+    )
+
+    repo_1 = github3.repos.Repository(
+        github_repo_metadata(
+            "auser", test_repo_data_one["name"], test_repo_data_one["id"]
+        ),
+        mock_api.session,
+    )
+    repo_1.hooks = MagicMock(return_value=[])
+    repo_1.file_contents = MagicMock(return_value=None)
+    # # Mock hook creation to retun the hook id '12345'
+    hook_instance = MagicMock()
+    hook_instance.id = 12345
+    repo_1.create_hook = MagicMock(return_value=hook_instance)
+
+    repo_2 = github3.repos.Repository(
+        github_repo_metadata(
+            "auser", test_repo_data_two["name"], test_repo_data_two["id"]
+        ),
+        mock_api.session,
+    )
+
+    repo_2.hooks = MagicMock(return_value=[])
+    repo_2.create_hook = MagicMock(return_value=hook_instance)
+
+    file_path = "test.py"
+
+    def mock_file_content():
+        # File contents mocking
+        owner = "auser"
+        repo = test_repo_data_two["name"]
+        ref = ""
+
+        # Dummy data to be encoded as the file contents
+        data = "dummy".encode("ascii")
+        return github_file_contents(owner, repo, file_path, ref, data)
+
+    file_data = mock_file_content()
+
+    def mock_file_contents(path, ref=None):
+        if path == file_path:
+            # Mock github3.contents.Content with file_data
+            return MagicMock(decoded=file_data)
+        return None
+
+    repo_2.file_contents = MagicMock(side_effect=mock_file_contents)
+
+    repo_3 = github3.repos.Repository(
+        fixtures.github_repo_metadata(
+            "auser", test_repo_data_three["name"], test_repo_data_three["id"]
+        ),
+        mock_api.session,
+    )
+    repo_3.hooks = MagicMock(return_value=[])
+    repo_3.file_contents = MagicMock(return_value=None)
+
+    repos = {1: repo_1, 2: repo_2, 3: repo_3}
+    repos_by_name = {r.full_name: r for r in repos.values()}
+    mock_api.repositories.return_value = repos.values()
+
+    def mock_repo_with_id(id):
+        return repos.get(id)
+
+    def mock_repo_by_name(owner, name):
+        return repos_by_name.get("/".join((owner, name)))
+
+    mock_api.repository_with_id.side_effect = mock_repo_with_id
+    mock_api.repository.side_effect = mock_repo_by_name
+    mock_api.markdown.side_effect = lambda x: x
+    mock_api.session.head.return_value = MagicMock(status_code=200)
+    mock_api.session.get.return_value = MagicMock(raw=fixtures.ZIPBALL())
+
+    with patch("invenio_github.api.GitHubAPI.api", new=mock_api):
+        with patch("invenio_github.api.GitHubAPI._sync_hooks"):
+            yield mock_api
```

### Comparing `invenio-github-1.0.0a9/invenio_github/__init__.py` & `invenio-github-1.0.0b1/invenio_github/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2012, 2013, 2014, 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -20,13 +20,12 @@
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
-from __future__ import absolute_import, print_function
-
 from .ext import InvenioGitHub
-from .version import __version__
 
-__all__ = ('__version__', 'InvenioGitHub')
+__version__ = "1.0.0b1"
+
+__all__ = ("__version__", "InvenioGitHub")
```

### Comparing `invenio-github-1.0.0a9/invenio_github/api.py` & `invenio-github-1.0.0b1/invenio_github/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2012, 2013, 2014, 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -20,32 +20,47 @@
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
+import json
+from contextlib import contextmanager
+
 import github3
+import humanize
+import requests
 from flask import current_app
+from invenio_access.permissions import authenticated_user
+from invenio_access.utils import get_identity
 from invenio_db import db
 from invenio_oauth2server.models import Token as ProviderToken
 from invenio_oauthclient.handlers import token_getter
 from invenio_oauthclient.models import RemoteAccount, RemoteToken
 from invenio_oauthclient.proxies import current_oauthclient
-from invenio_pidstore.proxies import current_pidstore
-from mistune import markdown
-from six import string_types
 from sqlalchemy.orm.exc import NoResultFound
 from werkzeug.local import LocalProxy
-from werkzeug.utils import cached_property, import_string
+from werkzeug.utils import cached_property
 
-from .errors import RepositoryAccessError
-from .models import Repository
-from .tasks import sync_hooks
-from .utils import get_extra_metadata, iso_utcnow, parse_timestamp, utcnow
+from .errors import (
+    RemoteAccountDataNotSet,
+    RemoteAccountNotFound,
+    RepositoryAccessError,
+    RepositoryNotFoundError,
+)
+from .models import ReleaseStatus, Repository
+from .tasks import sync_hooks as sync_hooks_task
+from .utils import iso_utcnow, parse_timestamp, utcnow
+
+
+def check_repo_access_permissions(repo, user_id, repo_id, repo_name):
+    """Checks permissions from user on repo."""
+    if repo and repo.user_id and repo.user_id != int(user_id):
+        raise RepositoryAccessError(user=user_id, repo=repo_name, repo_id=repo_id)
 
 
 class GitHubAPI(object):
     """Wrapper for GitHub API."""
 
     def __init__(self, user_id=None):
         """Create a GitHub API object."""
@@ -56,66 +71,73 @@
         """Return an authenticated GitHub API."""
         return github3.login(token=self.access_token)
 
     @cached_property
     def access_token(self):
         """Return OAuth access token."""
         if self.user_id:
-            return RemoteToken.get(
-                self.user_id, self.remote.consumer_key
-            ).access_token
+            return RemoteToken.get(self.user_id, self.remote.consumer_key).access_token
         return self.remote.get_request_token()[0]
 
     @property
     def session_token(self):
         """Return OAuth session token."""
         session_token = None
         if self.user_id is not None:
             session_token = token_getter(self.remote)
         if session_token:
             token = RemoteToken.get(
-                self.user_id, self.remote.consumer_key,
-                access_token=session_token[0]
+                self.user_id, self.remote.consumer_key, access_token=session_token[0]
             )
             return token
         return None
 
     remote = LocalProxy(
         lambda: current_oauthclient.oauth.remote_apps[
-            current_app.config['GITHUB_WEBHOOK_RECEIVER_ID']
+            current_app.config["GITHUB_WEBHOOK_RECEIVER_ID"]
         ]
     )
     """Return OAuth remote application."""
 
     @cached_property
     def account(self):
         """Return remote account."""
         return RemoteAccount.get(self.user_id, self.remote.consumer_key)
 
     @cached_property
     def webhook_url(self):
         """Return the url to be used by a GitHub webhook."""
+        if not self.account.extra_data.get("tokens", {}).get("webhook"):
+            raise RemoteAccountDataNotSet(
+                self.user_id, "Webhook data not found for user tokens (remote data)."
+            )
+
         webhook_token = ProviderToken.query.filter_by(
-            id=self.account.extra_data['tokens']['webhook']
+            id=self.account.extra_data["tokens"]["webhook"]
         ).first()
         if webhook_token:
-            wh_url = current_app.config.get('GITHUB_WEBHOOK_RECEIVER_URL')
+            wh_url = current_app.config.get("GITHUB_WEBHOOK_RECEIVER_URL")
             if wh_url:
                 return wh_url.format(token=webhook_token.access_token)
             else:
-                raise RuntimeError('You must set GITHUB_WEBHOOK_RECEIVER_URL.')
+                raise RuntimeError("You must set GITHUB_WEBHOOK_RECEIVER_URL.")
 
     def init_account(self):
         """Setup a new GitHub account."""
+        if not self.account:
+            raise RemoteAccountNotFound(
+                self.user_id, "Remote account was not found for user."
+            )
+
         ghuser = self.api.me()
         # Setup local access tokens to be used by the webhooks
         hook_token = ProviderToken.create_personal(
-            'github-webhook',
+            "github-webhook",
             self.user_id,
-            scopes=['webhooks:event'],
+            scopes=["webhooks:event"],
             is_internal=True,
         )
         # Initial structure of extra data
         self.account.extra_data = dict(
             id=ghuser.id,
             login=ghuser.login,
             name=ghuser.name,
@@ -123,326 +145,458 @@
                 webhook=hook_token.id,
             ),
             repos=dict(),
             last_sync=iso_utcnow(),
         )
         db.session.add(self.account)
 
-        # Sync data from GitHub, but don't check repository hooks yet.
-        self.sync(hooks=False)
-
     def sync(self, hooks=True, async_hooks=True):
         """Synchronize user repositories.
 
         :param bool hooks: True for syncing hooks.
         :param bool async_hooks: True for sending of an asynchronous task to
                                  sync hooks.
 
         .. note::
 
             Syncing happens from GitHub's direction only. This means that we
             consider the information on GitHub as valid, and we overwrite our
             own state based on this information.
         """
         active_repos = {}
-        github_repos = {repo.id: repo for repo in self.api.repositories()
-                        if repo.permissions['admin']}
+        github_repos = {
+            repo.id: repo
+            for repo in self.api.repositories()
+            if repo.permissions["admin"]
+        }
         for gh_repo_id, gh_repo in github_repos.items():
             active_repos[gh_repo_id] = {
-                'id': gh_repo_id,
-                'full_name': gh_repo.full_name,
-                'description': gh_repo.description,
+                "id": gh_repo_id,
+                "full_name": gh_repo.full_name,
+                "description": gh_repo.description,
+                "default_branch": gh_repo.default_branch,
             }
 
         if hooks:
-            self._sync_hooks(list(active_repos.keys()), async=async_hooks)
+            self._sync_hooks(list(active_repos.keys()), asynchronous=async_hooks)
+
+        # Update changed names for repositories stored in DB
+        db_repos = Repository.query.filter(
+            Repository.user_id == self.user_id,
+        )
+
+        for repo in db_repos:
+            if gh_repo and repo.name != gh_repo.full_name:
+                repo.name = gh_repo.full_name
+                db.session.add(repo)
 
         # Remove ownership from repositories that the user has no longer
         # 'admin' permissions, or have been deleted.
         Repository.query.filter(
             Repository.user_id == self.user_id,
-            ~Repository.github_id.in_(github_repos.keys())
         ).update(dict(user_id=None, hook=None), synchronize_session=False)
 
         # Update repos and last sync
-        self.account.extra_data.update(dict(
-            repos=active_repos,
-            last_sync=iso_utcnow(),
-        ))
+        self.account.extra_data.update(
+            dict(
+                repos=active_repos,
+                last_sync=iso_utcnow(),
+            )
+        )
         self.account.extra_data.changed()
         db.session.add(self.account)
 
-    def _sync_hooks(self, repos, async=True):
+    def _sync_hooks(self, repos, asynchronous=True):
         """Check if a hooks sync task needs to be started."""
-        if not async:
+        if not asynchronous:
             for repo_id in repos:
                 try:
-                    with db.session.begin_nested():
-                        self.sync_repo_hook(repo_id)
-                    db.session.commit()
-                except (NoResultFound, RepositoryAccessError) as e:
-                    current_app.logger.warning(e.message, exc_info=True)
+                    self.sync_repo_hook(repo_id)
+                except RepositoryAccessError:
+                    current_app.logger.warning(
+                        str(RepositoryAccessError), exc_info=True
+                    )
+                except NoResultFound:
+                    pass  # Repository not in DB yet
         else:
-            # FIXME: We have to commit, in order to have all necessary data?
+            # If hooks will run asynchronously, we need to commit any changes done so far
             db.session.commit()
-            sync_hooks.delay(self.user_id, repos)
+            sync_hooks_task.delay(self.user_id, repos)
 
     def sync_repo_hook(self, repo_id):
         """Sync a GitHub repo's hook with the locally stored repo."""
         # Get the hook that we may have set in the past
         gh_repo = self.api.repository_with_id(repo_id)
-        hooks = (hook.id for hook in gh_repo.hooks()
-                 if hook.config.get('url', '') == self.webhook_url)
-        hook_id = next(hooks, None)
+        hooks = (
+            hook
+            for hook in gh_repo.hooks()
+            if hook.config.get("url", "") == self.webhook_url
+        )
+        hook = next(hooks, None)
 
         # If hook on GitHub exists, get or create corresponding db object and
         # enable the hook. Otherwise remove the old hook information.
-        if hook_id:
-            Repository.enable(user_id=self.user_id,
-                              github_id=gh_repo.id,
-                              name=gh_repo.full_name,
-                              hook=hook_id)
+        repo = Repository.get(repo_id, gh_repo.full_name)
+        if not repo:
+            repo = Repository.create(self.user_id, repo_id, gh_repo.full_name)
+
+        if hook:
+            Repository.enable(repo, self.user_id, hook.id)
         else:
-            Repository.disable(user_id=self.user_id,
-                               github_id=gh_repo.id,
-                               name=gh_repo.full_name)
+            Repository.disable(repo)
 
     def check_sync(self):
         """Check if sync is required based on last sync date."""
         # If refresh interval is not specified, we should refresh every time.
         expiration = utcnow()
-        refresh_td = current_app.config.get('GITHUB_REFRESH_TIMEDELTA')
+        refresh_td = current_app.config.get("GITHUB_REFRESH_TIMEDELTA")
         if refresh_td:
             expiration -= refresh_td
-        last_sync = parse_timestamp(self.account.extra_data['last_sync'])
+        last_sync = parse_timestamp(self.account.extra_data["last_sync"])
         return last_sync < expiration
 
     def create_hook(self, repo_id, repo_name):
         """Create repository hook."""
-        config = dict(
+        # Get or create the repo and check access permissions
+        repo = Repository.get(github_id=repo_id, name=repo_name)
+        if not repo:
+            repo = Repository.create(self.user_id, repo_id, repo_name)
+
+        check_repo_access_permissions(
+            repo, self.user_id, repo_id=repo_id, repo_name=repo_name
+        )
+
+        # Create hook
+        hook_config = dict(
             url=self.webhook_url,
-            content_type='json',
-            secret=current_app.config['GITHUB_SHARED_SECRET'],
-            insecure_ssl='1' if current_app.config['GITHUB_INSECURE_SSL']
-                         else '0',
+            content_type="json",
+            secret=current_app.config["GITHUB_SHARED_SECRET"],
+            insecure_ssl="1" if current_app.config["GITHUB_INSECURE_SSL"] else "0",
         )
 
         ghrepo = self.api.repository_with_id(repo_id)
         if ghrepo:
-            try:
+            hooks = (
+                h
+                for h in ghrepo.hooks()
+                if h.config.get("url", "") == hook_config["url"]
+            )
+            hook = next(hooks, None)
+
+            # If hook does not exist, create one.
+            if not hook:
                 hook = ghrepo.create_hook(
-                    'web',  # GitHub identifier for webhook service
-                    config,
-                    events=['release'],
+                    "web",  # GitHub identifier for webhook service
+                    hook_config,
+                    events=["release"],
                 )
-            except github3.GitHubError as e:
-                # Check if hook is already installed
-                hook_errors = (m for m in e.errors
-                               if m['code'] == 'custom' and
-                               m['resource'] == 'Hook')
-                if next(hook_errors, None):
-                    hooks = (h for h in ghrepo.hooks()
-                             if h.config.get('url', '') == config['url'])
-                    hook = next(hooks, None)
-                    if hook:
-                        hook.edit(config=config, events=['release'])
-            finally:
-                if hook:
-                    Repository.enable(user_id=self.user_id,
-                                      github_id=repo_id,
-                                      name=repo_name,
-                                      hook=hook.id)
-                    return True
+            else:
+                hook.edit(config=hook_config, events=["release"])
+
+            Repository.enable(repo, self.user_id, hook.id)
+            return True
+
         return False
 
     def remove_hook(self, repo_id, name):
         """Remove repository hook."""
+        repo = Repository.get(github_id=repo_id, name=name)
+
+        if not repo:
+            raise RepositoryNotFoundError(repo_id)
+
+        check_repo_access_permissions(
+            repo, self.user_id, repo_id=repo_id, repo_name=name
+        )
+
         ghrepo = self.api.repository_with_id(repo_id)
         if ghrepo:
-            hooks = (h for h in ghrepo.hooks()
-                     if h.config.get('url', '') == self.webhook_url)
+            hooks = (
+                h for h in ghrepo.hooks() if h.config.get("url", "") == self.webhook_url
+            )
             hook = next(hooks, None)
             if not hook or hook.delete():
-                Repository.disable(user_id=self.user_id,
-                                   github_id=repo_id,
-                                   name=name)
+                Repository.disable(repo)
                 return True
         return False
 
+    def get_repository_releases(self, repo_name="", repo=None):
+        """Retrieve repository releases."""
+        if not (repo or repo_name):
+            raise ValueError("At least one of (repo, repo_name) is required")
+
+        if not repo:
+            repo = Repository.get(name=repo_name)
+
+        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo_name)
+
+        # Retrieve releases and sort them by creation date
+        release_objects = sorted(repo.releases.all(), key=lambda r: r.created)
+
+        return release_objects
+
+    def get_user_repositories(self):
+        """Retrieves user repositories."""
+        token = self.session_token
+        if token:
+            extra_data = self.account.extra_data
+        repos = extra_data.get("repos", [])
+        if repos:
+            # 'Enhance' our repos dict, from our database model
+            db_repos = Repository.query.filter(
+                Repository.github_id.in_([int(k) for k in repos.keys()]),
+            ).all()
+            for repo in db_repos:
+                repos[str(repo.github_id)]["instance"] = repo
+                repos[str(repo.github_id)]["latest"] = GitHubRelease(
+                    repo.latest_release()
+                )
+        return repos
+
+    def get_last_sync_time(self):
+        """Retrieves the last sync delta time from github's client extra data.
+
+        Time is computed as the delta between now and the last sync time.
+        """
+        if not self.account.extra_data.get("last_sync"):
+            raise RemoteAccountDataNotSet(
+                self.user_id, "Last sync data is not set for user (remote data)."
+            )
+
+        extra_data = self.account.extra_data
+        last_sync = humanize.naturaltime(
+            (utcnow() - parse_timestamp(extra_data["last_sync"]))
+        )
+        return last_sync
+
+    def get_repository(self, repo_name):
+        """Retrieves one repository.
+
+        Checks for access permission.
+        """
+        repo = Repository.get(name=repo_name)
+        if not repo:
+            raise RepositoryNotFoundError(repo_name)
+
+        # Might raise a RepositoryAccessError
+        check_repo_access_permissions(repo, self.user_id, repo.github_id, repo_name)
+
+        return repo
+
     @classmethod
     def _dev_api(cls):
         """Get a developer instance for GitHub API access."""
         gh = github3.GitHub()
         gh.set_client_id(cls.remote.consumer_key, cls.remote.consumer_secret)
         return gh
 
     @classmethod
     def check_token(cls, token):
         """Check if an access token is authorized."""
-        return cls._dev_api().check_authorization(token)
+        gh_api = cls._dev_api()
+        client_id, client_secret = gh_api.session.retrieve_client_credentials()
+        url = gh_api._build_url("applications", str(client_id), "token")
+        with gh_api.session.temporary_basic_auth(client_id, client_secret):
+            response = gh_api._post(url, data={"access_token": token})
+        return response.status_code == 200
 
     @classmethod
     def revoke_token(cls, token):
         """Revoke an access token."""
-        return cls._dev_api().revoke_authorization(token)
+        gh_api = cls._dev_api()
+        client_id, client_secret = gh_api.session.retrieve_client_credentials()
+        url = gh_api._build_url("applications", str(client_id), "token")
+        with gh_api.session.temporary_basic_auth(client_id, client_secret):
+            response = gh_api._delete(url, data=json.dumps({"access_token": token}))
+        return response
 
 
 class GitHubRelease(object):
     """A GitHub release."""
 
     def __init__(self, release):
         """Constructor."""
-        self.model = release
+        self.release_object = release
+
+    @cached_property
+    def record(self):
+        """Release record."""
+        return self.resolve_record()
 
     @cached_property
     def gh(self):
         """Return GitHubAPI object."""
         return GitHubAPI(user_id=self.event.user_id)
 
     @cached_property
-    def deposit_class(self):
-        """Return a class implementing `publish` method."""
-        cls = current_app.config['GITHUB_DEPOSIT_CLASS']
-        if isinstance(cls, string_types):
-            cls = import_string(cls)
-        assert isinstance(cls, type)
-        return cls
-
-    @cached_property
     def event(self):
         """Get release event."""
-        return self.model.event
+        return self.release_object.event
 
     @cached_property
     def payload(self):
         """Return event payload."""
         return self.event.payload
 
     @cached_property
-    def release(self):
+    def release_payload(self):
         """Return release metadata."""
-        return self.payload['release']
+        return self.payload["release"]
 
     @cached_property
-    def repository(self):
+    def repository_payload(self):
         """Return repository metadata."""
-        return self.payload['repository']
-
-    @property
-    def repo_model(self):
-        """Return repository model from database."""
-        return Repository.query.filter_by(
-            user_id=self.event.user_id,
-            github_id=self.repository['id'],
-        ).one()
+        return self.payload["repository"]
 
     @cached_property
-    def title(self):
-        """Extract title from a release."""
-        if self.event:
-            if self.release['name']:
-                return u'{0}: {1}'.format(
-                    self.repository['full_name'], self.release['name']
+    def repository_object(self):
+        """Return repository model from database."""
+        if self.release_object.repository_id:
+            repository = self.release_object.repository
+        else:
+            repository = Repository.query.filter_by(
+                user_id=self.event.user_id,
+            ).one()
+        return repository
+
+    @cached_property
+    def release_file_name(self):
+        """Returns release zipball file name."""
+        tag_name = self.release_payload["tag_name"]
+        repo_name = self.repository_payload["full_name"]
+        filename = f"{repo_name}-{tag_name}.zip"
+        return filename
+
+    @cached_property
+    def release_zipball_url(self):
+        """Returns the release zipball url."""
+        return self.release_payload["zipball_url"]
+
+    @cached_property
+    def user_identity(self):
+        """Generates release owner's user identity."""
+        identity = get_identity(self.repository_object.user)
+        identity.provides.add(authenticated_user)
+        identity.user = self.repository_object.user
+        return identity
+
+    @cached_property
+    def contributors(self):
+        """Get list of contributors to a repository."""
+        try:
+            contributors_iter = self.gh.api.repository_with_id(
+                self.repository_object.github_id
+            ).contributors()
+            contributors = list(contributors_iter)
+            if contributors_iter.last_status == 200:
+
+                def get_author(contributor):
+                    r = requests.get(contributor["url"])
+                    if r.status_code == 200:
+                        data = r.json()
+                        return data
+
+                # Sort according to number of contributions
+                contributors = sorted(
+                    contributors,
+                    key=lambda x: x.as_dict()["contributions"],
+                    reverse=True,
                 )
-        return u'{0} {1}'.format(self.repo_model.name, self.model.tag)
-
-    @cached_property
-    def description(self):
-        """Extract description from a release."""
-        if self.release.get('body'):
-            return markdown(self.release['body'])
-        elif self.repository.get('description'):
-            return self.repository['description']
-        return 'No description provided.'
-
-    @cached_property
-    def author(self):
-        """Extract the author's GitHub username from a release."""
-        return self.release.get('author', {}).get('login')
-
-    @cached_property
-    def related_identifiers(self):
-        """Yield related identifiers."""
-        yield dict(
-            identifier='https://github.com/{0}/tree/{1}'.format(
-                self.repository['full_name'], self.release['tag_name']
-            ),
-            relation='isSupplementTo',
-        )
-
-    @cached_property
-    def defaults(self):
-        """Return default metadata."""
-        return dict(
-            access_right='open',
-            description=self.description,
-            license='other-open',
-            publication_date=self.release['published_at'][:10],
-            related_identifiers=list(self.related_identifiers),
-            title=self.title,
-            upload_type='software',
-        )
-
-    @cached_property
-    def extra_metadata(self):
-        """Get extra metadata for file in repository."""
-        return get_extra_metadata(
-            self.gh.api,
-            self.repository['owner']['login'],
-            self.repository['name'],
-            self.release['tag_name'],
-        )
+                max_contributors = current_app.config.get(
+                    "GITHUB_MAX_CONTRIBUTORS_NUMBER", 30
+                )
+                contributors = [
+                    get_author(x.as_dict())
+                    for x in contributors[:max_contributors]
+                    if x.as_dict()["type"] == "User"
+                ]
+                contributors = filter(lambda x: x is not None, contributors)
+                return list(contributors)
+        except Exception:
+            return None
+
+    # Helper functions
+
+    def is_first_release(self):
+        """Checks whether the current release is the first release of the repository."""
+        latest_release = self.repository_object.latest_release(ReleaseStatus.PUBLISHED)
+        return True if not latest_release else False
 
-    @cached_property
-    def files(self):
+    def test_zipball(self):
         """Extract files to download from GitHub payload."""
-        tag_name = self.release['tag_name']
-        repo_name = self.repository['full_name']
-
-        zipball_url = self.release['zipball_url']
-        filename = '{name}-{tag}.zip'.format(name=repo_name, tag=tag_name)
+        zipball_url = self.release_payload["zipball_url"]
 
-        response = self.gh.api.session.head(zipball_url)
-        assert response.status_code == 302, \
-            'Could not retrieve archive from GitHub: {0}'.format(zipball_url)
+        # Execute a HEAD request to the zipball url to test the url.
+        response = self.gh.api.session.head(zipball_url, allow_redirects=True)
 
-        yield filename, zipball_url
+        # In case where there is a tag and branch with the same name, we might
+        # get back a "300 Mutliple Choices" response, which requires fetching
+        # an "alternate" link.
+        if response.status_code == 300:
+            zipball_url = response.links.get("alternate", {}).get("url")
+            if zipball_url:
+                response = self.gh.api.session.head(zipball_url, allow_redirects=True)
+                # Another edge-case, is when the access token we have does not
+                # have the scopes/permissions to access public links. In that
+                # rare case we fallback to a non-authenticated request.
+                if response.status_code == 404:
+                    response = requests.head(zipball_url, allow_redirects=True)
+                    # If this response is successful we want to use the finally
+                    # resolved URL to fetch the ZIP from.
+                    if response.status_code == 200:
+                        zipball_url = response.url
+
+        assert (
+            response.status_code == 200
+        ), f"Could not retrieve archive from GitHub: {zipball_url}"
+
+    # High level API
+
+    # TODO split maybe
+    def release_failed(self):
+        """Set release status to FAILED."""
+        self.release_object.status = ReleaseStatus.FAILED
+
+    def release_processing(self):
+        """Set release status to PROCESSING."""
+        self.release_object.status = ReleaseStatus.PROCESSING
+
+    def release_published(self):
+        """Set release status to PUBLISHED."""
+        self.release_object.status = ReleaseStatus.PUBLISHED
 
-    @property
-    def metadata(self):
-        """Return extracted metadata."""
-        output = dict(self.defaults)
-        output.update(self.extra_metadata)
-        return output
+    def retrieve_remote_file(self, file_name):
+        """Retrieves a file from the repository, for the current release, using the github client.
 
-    @cached_property
-    def record(self):
-        """Get Release record."""
-        return self.model.record
-
-    @cached_property
-    def pid(self):
-        """Get PID object for the Release record."""
-        if self.record:
-            fetcher = current_pidstore.fetchers[
-                current_app.config.get('GITHUB_PID_FETCHER')]
-            return fetcher(self.record.id, self.record)
-
-    def verify_sender(self):
-        """Check if the sender is valid."""
-        return self.payload['repository']['full_name'] in \
-            self.gh.account.extra_data['repos']
+        :param file_name: the name of the file to be retrieved from the repository.
+        :returns: the file contents or None, if the file if not fetched.
+        """
+        gh_repo_owner = self.repository_payload["owner"]["login"]
+        gh_repo_name = self.repository_payload["name"]
+        gh_tag_name = self.release_payload["tag_name"]
+        try:
+            content = self.gh.api.repository(gh_repo_owner, gh_repo_name).file_contents(
+                path=file_name, ref=gh_tag_name
+            )
+        except github3.exceptions.NotFoundError:
+            # github3 raises a github3.exceptions.NotFoundError if the file is not found
+            return None
+        return content
+
+    @contextmanager
+    def fetch_zipball_file(self):
+        """Fetch release zipball file using the current github session."""
+        session = self.gh.api.session
+        with session.get(self.release_zipball_url, stream=True) as s:
+            yield s.raw
 
     def publish(self):
-        """Publish GitHub release as record."""
-        with db.session.begin_nested():
-            deposit = self.deposit_class.create(self.metadata)
-            deposit['_deposit']['created_by'] = self.event.user_id
-            deposit['_deposit']['owners'] = [self.event.user_id]
-
-            # Fetch the deposit files
-            for key, url in self.files:
-                deposit.files[key] = self.gh.api.session.get(
-                    url, stream=True).raw
+        """Publish a GitHub release."""
+        raise NotImplementedError
 
-            deposit.publish()
-            self.model.recordmetadata = deposit.model
+    def process_release(self):
+        """Processes a github release."""
+        raise NotImplementedError
+
+    def resolve_record(self):
+        """Resolves a record from the release. To be implemented by the API class implementation."""
+        raise NotImplementedError
```

### Comparing `invenio-github-1.0.0a9/invenio_github/config.py` & `invenio-github-1.0.0b1/invenio_github/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be useful,
@@ -23,15 +23,15 @@
 """Configuration for GitHub module."""
 
 from copy import deepcopy
 from datetime import timedelta
 
 from invenio_oauthclient.contrib.github import REMOTE_APP
 
-GITHUB_WEBHOOK_RECEIVER_ID = 'github'
+GITHUB_WEBHOOK_RECEIVER_ID = "github"
 """Local name of webhook receiver."""
 
 GITHUB_WEBHOOK_RECEIVER_URL = None
 """URL format to be used when creating a webhook on GitHub.
 
 This configuration variable must be set explicitly. Example::
 
@@ -40,15 +40,15 @@
 .. note::
 
     This config variable is used because using `url_for` to get and external
     url of an `invenio_base.api_bluebrint`, while inside the regular app
     context, doesn't work as expected.
 """
 
-GITHUB_SHARED_SECRET = 'CHANGEME'
+GITHUB_SHARED_SECRET = "CHANGEME"
 """Shared secret between you and GitHub.
 
 Used to make GitHub sign webhook requests with HMAC.
 
 See http://developer.github.com/v3/repos/hooks/#example
 """
 
@@ -58,37 +58,26 @@
 Never set to True in a production environment, but can be useful for
 development and integration servers.
 """
 
 GITHUB_REFRESH_TIMEDELTA = timedelta(days=1)
 """Time period after which a GitHub account sync should be initiated."""
 
-GITHUB_RELEASE_CLASS = 'invenio_github.api:GitHubRelease'
+GITHUB_RELEASE_CLASS = "invenio_github.api:GitHubRelease"
 """GitHubRelease class to be used for release handling."""
 
-GITHUB_METADATA_FILE = '.invenio.json'
-"""File with extra metadata stored in GitHub repository."""
-
-GITHUB_DEPOSIT_CLASS = 'invenio_deposit.api:Deposit'
-"""Deposit class that implements a `publish` method."""
-
-GITHUB_RECORD_SERIALIZER = None
-"""Serializer to use to display record metadata."""
-
-GITHUB_PID_FETCHER = 'recid'
-"""PID Fetcher for Release records."""
-
-GITHUB_TEMPLATE_INDEX = 'invenio_github/settings/index.html'
+GITHUB_TEMPLATE_INDEX = "invenio_github/settings/index.html"
 """Repositories list template."""
 
-GITHUB_TEMPLATE_VIEW = 'invenio_github/settings/view.html'
+GITHUB_TEMPLATE_VIEW = "invenio_github/settings/view.html"
 """Repository detail view template."""
 
-# Copy the default GitHub OAuth application configuration, and update
-# handlers and scope.
-GITHUB_REMOTE_APP = deepcopy(REMOTE_APP)
+GITHUB_ERROR_HANDLERS = None
+"""Definition of the way specific exceptions are handled."""
+
+GITHUB_MAX_CONTRIBUTORS_NUMBER = 30
+"""Max number of contributors of a release to be retrieved from Github."""
+
+# Copy the default GitHub OAuth application configuration, and update disconnect handlers and scope.
 """OAuth Client configuration."""
-GITHUB_REMOTE_APP['disconnect_handler'] = 'invenio_github.handlers:disconnect'
-GITHUB_REMOTE_APP['signup_handler']['setup'] = \
-    'invenio_github.handlers:account_setup'
-GITHUB_REMOTE_APP['params']['request_token_params']['scope'] = \
-    'user,admin:repo_hook,read:org'
+REMOTE_APP["disconnect_handler"] = "invenio_github.handlers:disconnect"
+REMOTE_APP["params"]["request_token_params"]["scope"] = "user,admin:repo_hook,read:org"
```

### Comparing `invenio-github-1.0.0a9/invenio_github/errors.py` & `invenio-github-1.0.0b1/tests/test_models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,30 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
-# Invenio is free software; you can redistribute it
-# and/or modify it under the terms of the GNU General Public License as
-# published by the Free Software Foundation; either version 2 of the
-# License, or (at your option) any later version.
+# Invenio is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
-# Invenio is distributed in the hope that it will be
-# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# Invenio is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with Invenio; if not, write to the
-# Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
-# MA 02111-1307, USA.
+# along with Invenio. If not, see <http://www.gnu.org/licenses/>.
 #
-# In applying this license, CERN does not
-# waive the privileges and immunities granted to it by virtue of its status
-# as an Intergovernmental Organization or submit itself to any jurisdiction.
+# In applying this licence, CERN does not waive the privileges and immunities
+# granted to it by virtue of its status as an Intergovernmental Organization
+# or submit itself to any jurisdiction.
 
-"""Invenio-GitHub errors."""
+"""Test cases for badge creation."""
 
+from invenio_github.models import Repository
 
-class GitHubError(Exception):
-    """General GitHub error."""
 
-
-class RepositoryAccessError(GitHubError):
-    """Repository access permissions error."""
-
-
-class RepositoryDisabledError(GitHubError):
-    """Repository access permissions error."""
-
-
-class InvalidSenderError(GitHubError):
-    """Invalid release sender error."""
-
-
-class ReleaseAlreadyReceivedError(GitHubError):
-    """Invalid release sender error."""
-
-
-class CustomGitHubMetadataError(GitHubError):
-    """Invalid Custom GitHub Metadata file."""
+def test_repository_unbound(app):
+    """Test create_badge method."""
+    assert Repository(name="org/repo", github_id=1).latest_release() is None
```

### Comparing `invenio-github-1.0.0a9/invenio_github/ext.py` & `invenio-github-1.0.0b1/invenio_github/ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -20,82 +20,82 @@
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
-from __future__ import absolute_import, print_function
-
 from flask import current_app
 from six import string_types
 from sqlalchemy import event
 from werkzeug.utils import cached_property, import_string
 
 from . import config
 from .api import GitHubRelease
+from .utils import obj_or_import_string
 
 
 class InvenioGitHub(object):
     """Invenio-GitHub extension."""
 
     def __init__(self, app=None):
         """Extension initialization."""
         if app:
             self.init_app(app)
 
     @cached_property
     def release_api_class(self):
         """Github Release API class."""
-        cls = current_app.config['GITHUB_RELEASE_CLASS']
+        cls = current_app.config["GITHUB_RELEASE_CLASS"]
         if isinstance(cls, string_types):
             cls = import_string(cls)
         assert issubclass(cls, GitHubRelease)
         return cls
 
     @cached_property
-    def record_serializer(self):
-        """Github Release API class."""
-        imp = current_app.config['GITHUB_RECORD_SERIALIZER']
-        if isinstance(imp, string_types):
-            return import_string(imp)
-        return imp
+    def release_error_handlers(self):
+        """Github Release error handlers."""
+        error_handlers = current_app.config.get("GITHUB_ERROR_HANDLERS") or []
+        return [
+            (obj_or_import_string(error_cls), obj_or_import_string(handler))
+            for error_cls, handler in error_handlers
+        ]
 
     def init_app(self, app):
         """Flask application initialization."""
         self.init_config(app)
-        app.extensions['invenio-github'] = self
+        app.extensions["invenio-github"] = self
 
         @app.before_first_request
         def connect_signals():
             """Connect OAuthClient signals."""
             from invenio_oauthclient.models import RemoteAccount
             from invenio_oauthclient.signals import account_setup_committed
 
             from .api import GitHubAPI
             from .handlers import account_post_init
 
             account_setup_committed.connect(
-                account_post_init,
-                sender=GitHubAPI.remote._get_current_object()
+                account_post_init, sender=GitHubAPI.remote._get_current_object()
             )
 
-            @event.listens_for(RemoteAccount, 'before_delete')
+            @event.listens_for(RemoteAccount, "before_delete")
             def receive_before_delete(mapper, connection, target):
                 """Listen for the 'before_delete' event."""
-                # TODO remove hooks
 
     def init_config(self, app):
         """Initialize configuration."""
         app.config.setdefault(
-            'GITHUB_BASE_TEMPLATE',
-            app.config.get('BASE_TEMPLATE',
-                           'invenio_github/base.html'))
+            "GITHUB_BASE_TEMPLATE",
+            app.config.get("BASE_TEMPLATE", "invenio_github/base.html"),
+        )
 
         app.config.setdefault(
-            'GITHUB_SETTINGS_TEMPLATE',
-            app.config.get('SETTINGS_TEMPLATE',
-                           'invenio_oauth2server/settings/base.html'))
+            "GITHUB_SETTINGS_TEMPLATE",
+            app.config.get(
+                "SETTINGS_TEMPLATE", "invenio_oauth2server/settings/base.html"
+            ),
+        )
 
         for k in dir(config):
-            if k.startswith('GITHUB_'):
+            if k.startswith("GITHUB_"):
                 app.config.setdefault(k, getattr(config, k))
```

### Comparing `invenio-github-1.0.0a9/invenio_github/handlers.py` & `invenio-github-1.0.0b1/invenio_github/handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2014, 2015, 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be useful,
@@ -18,86 +18,69 @@
 #
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
 
 """Implement OAuth client handler."""
 
-from __future__ import absolute_import
-
 from flask import current_app, redirect, url_for
 from flask_login import current_user
 from invenio_db import db
 from invenio_oauth2server.models import Token as ProviderToken
 from invenio_oauthclient.models import RemoteToken
-from invenio_oauthclient.utils import oauth_link_external_id, \
-    oauth_unlink_external_id
+from invenio_oauthclient.utils import oauth_link_external_id, oauth_unlink_external_id
 from sqlalchemy.orm.exc import NoResultFound
 
 from .api import GitHubAPI
 from .models import Repository
-from .tasks import disconnect_github, sync_hooks
-
-
-def account_setup(remote, token=None, response=None,
-                  account_setup=None):
-    """Setup user account."""
-    gh = GitHubAPI(user_id=token.remote_account.user_id)
-    with db.session.begin_nested():
-        gh.init_account()
-
-        # Create user <-> external id link.
-        oauth_link_external_id(
-            token.remote_account.user,
-            dict(id=str(gh.account.extra_data['id']), method="github")
-        )
+from .tasks import disconnect_github
 
 
 def account_post_init(remote, token=None):
     """Perform post initialization."""
-    gh = GitHubAPI(user_id=token.remote_account.user_id)
-    repos = [r.id for r in gh.api.repositories() if r.permissions['admin']]
-    sync_hooks.delay(token.remote_account.user_id, repos)
+    try:
+        gh = GitHubAPI(user_id=token.remote_account.user_id)
+        gh.init_account()
+        gh.sync()
+        db.session.commit()
+    except Exception as e:
+        current_app.logger.warning(str(e), exc_info=True)
 
 
 def disconnect(remote):
     """Disconnect callback handler for GitHub."""
     # User must be authenticated
     if not current_user.is_authenticated:
         return current_app.login_manager.unauthorized()
 
-    external_method = 'github'
-    external_ids = [i.id for i in current_user.external_identifiers
-                    if i.method == external_method]
+    external_method = "github"
+    external_ids = [
+        i.id for i in current_user.external_identifiers if i.method == external_method
+    ]
     if external_ids:
-        oauth_unlink_external_id(dict(id=external_ids[0],
-                                      method=external_method))
+        oauth_unlink_external_id(dict(id=external_ids[0], method=external_method))
 
-    user_id = current_user.get_id()
+    user_id = int(current_user.get_id())
     token = RemoteToken.get(user_id, remote.consumer_key)
     if token:
         extra_data = token.remote_account.extra_data
 
         # Delete the token that we issued for GitHub to deliver webhooks
-        webhook_token_id = extra_data.get('tokens', {}).get('webhook')
+        webhook_token_id = extra_data.get("tokens", {}).get("webhook")
         ProviderToken.query.filter_by(id=webhook_token_id).delete()
 
         # Disable GitHub webhooks from our side
         db_repos = Repository.query.filter_by(user_id=user_id).all()
         # Keep repositories with hooks to pass to the celery task later on
         repos_with_hooks = [(r.github_id, r.hook) for r in db_repos if r.hook]
         for repo in db_repos:
-            try:
-                Repository.disable(user_id=user_id,
-                                   github_id=repo.github_id,
-                                   name=repo.name)
-            except NoResultFound:
-                # If the repository doesn't exist, no action is necessary
-                pass
+            Repository.disable(repo)
+        # Commit any changes before running the ascynhronous task
         db.session.commit()
 
         # Send Celery task for webhooks removal and token revocation
         disconnect_github.delay(token.access_token, repos_with_hooks)
         # Delete the RemoteAccount (along with the associated RemoteToken)
         token.remote_account.delete()
+        db.session.commit()
 
-    return redirect(url_for('invenio_oauthclient_settings.index'))
+    return redirect(url_for("invenio_oauthclient_settings.index"))
```

### Comparing `invenio-github-1.0.0a9/invenio_github/models.py` & `invenio-github-1.0.0b1/invenio_github/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -20,73 +20,70 @@
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Models for GitHub integration."""
 
-from __future__ import absolute_import
-
 import uuid
 from enum import Enum
 
-from flask import current_app
-from flask_babelex import lazy_gettext as _
 from invenio_accounts.models import User
 from invenio_db import db
-from invenio_records.api import Record
-from invenio_records.models import RecordMetadata
+from invenio_i18n import lazy_gettext as _
 from invenio_webhooks.models import Event
 from sqlalchemy.dialects import postgresql
-from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy_utils.models import Timestamp
 from sqlalchemy_utils.types import ChoiceType, JSONType, UUIDType
 
-from .errors import ReleaseAlreadyReceivedError, RepositoryAccessError, \
-    RepositoryDisabledError
-
 RELEASE_STATUS_TITLES = {
-    'RECEIVED': _('Received'),
-    'PROCESSING': _('Processing'),
-    'PUBLISHED': _('Published'),
-    'FAILED': _('Failed'),
+    "RECEIVED": _("Received"),
+    "PROCESSING": _("Processing"),
+    "PUBLISHED": _("Published"),
+    "FAILED": _("Failed"),
+    "DELETED": _("Deleted"),
 }
 
 RELEASE_STATUS_ICON = {
-    'RECEIVED': 'fa-spinner',
-    'PROCESSING': 'fa-spinner',
-    'PUBLISHED': 'fa-check',
-    'FAILED': 'fa-times',
+    "RECEIVED": "fa-spinner",
+    "PROCESSING": "fa-spinner",
+    "PUBLISHED": "fa-check",
+    "FAILED": "fa-times",
+    "DELETED": "fa-times",
 }
 
 RELEASE_STATUS_COLOR = {
-    'RECEIVED': 'default',
-    'PROCESSING': 'default',
-    'PUBLISHED': 'success',
-    'FAILED': 'danger',
+    "RECEIVED": "default",
+    "PROCESSING": "default",
+    "PUBLISHED": "success",
+    "FAILED": "danger",
+    "DELETED": "danger",
 }
 
 
 class ReleaseStatus(Enum):
     """Constants for possible status of a Release."""
 
-    __order__ = 'RECEIVED PROCESSING PUBLISHED FAILED'
+    __order__ = "RECEIVED PROCESSING PUBLISHED FAILED DELETED"
 
-    RECEIVED = 'R'
+    RECEIVED = "R"
     """Release has been received and is pending processing."""
 
-    PROCESSING = 'P'
+    PROCESSING = "P"
     """Release is still being processed."""
 
-    PUBLISHED = 'D'
+    PUBLISHED = "D"
     """Release was successfully processed and published."""
 
-    FAILED = 'F'
+    FAILED = "F"
     """Release processing has failed."""
 
+    DELETED = "E"
+    """Release has been deleted."""
+
     def __init__(self, value):
         """Hack."""
 
     def __eq__(self, other):
         """Equality test."""
         return self.value == other
 
@@ -109,15 +106,15 @@
         """UI status color."""
         return RELEASE_STATUS_COLOR[self.name]
 
 
 class Repository(db.Model, Timestamp):
     """Information about a GitHub repository."""
 
-    __tablename__ = 'github_repositories'
+    __tablename__ = "github_repositories"
 
     id = db.Column(
         UUIDType,
         primary_key=True,
         default=uuid.uuid4,
     )
     """Repository identifier."""
@@ -147,116 +144,101 @@
 
     name = db.Column(db.String(255), unique=True, index=True, nullable=False)
     """Fully qualified name of the repository including user/organization."""
 
     user_id = db.Column(db.Integer, db.ForeignKey(User.id), nullable=True)
     """Reference user that can manage this repository."""
 
-    ping = db.Column(db.DateTime, nullable=True)
-    """Last ping of the repository."""
-
     hook = db.Column(db.Integer)
     """Hook identifier."""
 
     #
     # Relationships
     #
     user = db.relationship(User)
 
     @classmethod
     def create(cls, user_id, github_id=None, name=None, **kwargs):
         """Create the repository."""
-        with db.session.begin_nested():
-            obj = cls(user_id=user_id, github_id=github_id, name=name,
-                      **kwargs)
-            db.session.add(obj)
+        obj = cls(user_id=user_id, github_id=github_id, name=name, **kwargs)
+        db.session.add(obj)
         return obj
 
     @classmethod
-    def get(cls, user_id, github_id=None, name=None, check_owner=True):
-        """Return a repository.
+    def get(cls, github_id=None, name=None):
+        """Return a repository given its name or github id.
 
-        :param integer user_id: User identifier.
         :param integer github_id: GitHub repository identifier.
         :param str name: GitHub repository full name.
         :returns: The repository object.
         :raises: :py:exc:`~sqlalchemy.orm.exc.NoResultFound`: if the repository
                  doesn't exist.
         :raises: :py:exc:`~sqlalchemy.orm.exc.MultipleResultsFound`: if
                  multiple repositories with the specified GitHub id and/or name
                  exist.
-        :raises: :py:exc:`RepositoryAccessError`: if the user is not the owner
-                 of the repository.
         """
-        repo = cls.query.filter((Repository.github_id == github_id) |
-                                (Repository.name == name)).one()
-        if check_owner and repo and repo.user_id and repo.user_id != user_id:
-            raise RepositoryAccessError(
-                'User {user} cannot access repository {repo}({repo_id}).'
-                .format(user=user_id, repo=name, repo_id=github_id)
-            )
+        repo = cls.query.filter(
+            (Repository.github_id == github_id) | (Repository.name == name)
+        ).one_or_none()
         return repo
 
     @classmethod
-    def enable(cls, user_id, github_id, name, hook):
+    def enable(cls, repo, user_id, hook):
         """Enable webhooks for a repository.
 
         If the repository does not exist it will create one.
 
         :param user_id: User identifier.
         :param repo_id: GitHub repository identifier.
         :param name: Fully qualified name of the repository.
-        :param hook: GitHub hook identifier.
+        :param hook: GitHub hook identifier (hook id).
         """
-        try:
-            repo = cls.get(user_id, github_id=github_id, name=name)
-        except NoResultFound:
-            repo = cls.create(user_id=user_id, github_id=github_id, name=name)
         repo.hook = hook
         repo.user_id = user_id
+        db.session.add(repo)
         return repo
 
     @classmethod
-    def disable(cls, user_id, github_id, name):
+    def disable(cls, repo):
         """Disable webhooks for a repository.
 
         Disables the webhook from a repository if it exists in the DB.
 
         :param user_id: User identifier.
         :param repo_id: GitHub id of the repository.
         :param name: Fully qualified name of the repository.
         """
-        repo = cls.get(user_id, github_id=github_id, name=name)
         repo.hook = None
         repo.user_id = None
+        db.session.add(repo)
         return repo
 
     @property
     def enabled(self):
         """Return if the repository has webhooks enabled."""
         return bool(self.hook)
 
     def latest_release(self, status=None):
         """Chronologically latest published release of the repository."""
-        # Bail out fast if object not in DB session.
+        # Bail out fast if object (Repository) not in DB session.
         if self not in db.session:
             return None
-        q = self.releases if status is None else self.releases.filter_by(
-            status=status)
+
+        q = self.releases if status is None else self.releases.filter_by(status=status)
         return q.order_by(db.desc(Release.created)).first()
 
     def __repr__(self):
         """Get repository representation."""
-        return '<Repository {self.name}:{self.github_id}>'.format(self=self)
+        return "<Repository {self.name}:{self.github_id}>".format(self=self)
 
 
 class Release(db.Model, Timestamp):
     """Information about a GitHub release."""
 
-    __tablename__ = 'github_releases'
+    __tablename__ = "github_releases"
 
     id = db.Column(
         UUIDType,
         primary_key=True,
         default=uuid.uuid4,
     )
     """Release identifier."""
@@ -265,98 +247,43 @@
     """Unique GitHub release identifier."""
 
     tag = db.Column(db.String(255))
     """Release tag."""
 
     errors = db.Column(
         JSONType().with_variant(
+            # TODO postgresql specific. Limits the usage of the DB engine.
             postgresql.JSON(none_as_null=True),
-            'postgresql',
+            "postgresql",
         ),
         nullable=True,
     )
     """Release processing errors."""
 
     repository_id = db.Column(UUIDType, db.ForeignKey(Repository.id))
     """Repository identifier."""
 
     event_id = db.Column(UUIDType, db.ForeignKey(Event.id), nullable=True)
     """Incoming webhook event identifier."""
 
     record_id = db.Column(
         UUIDType,
-        db.ForeignKey(RecordMetadata.id),
+        index=True,
         nullable=True,
     )
-    """Record identifier."""
+    """Weak reference to a record identifier."""
 
     status = db.Column(
         ChoiceType(ReleaseStatus, impl=db.CHAR(1)),
         nullable=False,
     )
     """Status of the release, e.g. 'processing', 'published', 'failed', etc."""
 
     repository = db.relationship(
-        Repository,
-        backref=db.backref('releases', lazy='dynamic')
+        Repository, backref=db.backref("releases", lazy="dynamic")
     )
 
-    recordmetadata = db.relationship(RecordMetadata)
     event = db.relationship(Event)
 
-    @classmethod
-    def create(cls, event):
-        """Create a new Release model."""
-        # Check if the release has already been received
-        release_id = event.payload['release']['id']
-        existing_release = Release.query.filter_by(
-            release_id=release_id,
-        ).first()
-        if existing_release:
-            raise ReleaseAlreadyReceivedError(
-                '{release} has already been received.'
-                .format(release=existing_release)
-            )
-
-        # Create the Release
-        repo_id = event.payload['repository']['id']
-        repo = Repository.get(user_id=event.user_id, github_id=repo_id)
-        if repo.enabled:
-            with db.session.begin_nested():
-                release = cls(
-                    release_id=release_id,
-                    tag=event.payload['release']['tag_name'],
-                    repository=repo,
-                    event=event,
-                    status=ReleaseStatus.RECEIVED,
-                )
-                db.session.add(release)
-            return release
-        else:
-            current_app.logger.warning(
-                'Release creation attempt on disabled {repo}.'
-                .format(repo=repo)
-            )
-            raise RepositoryDisabledError(
-                '{repo} is not enabled for webhooks.'.format(repo=repo)
-            )
-
-    @property
-    def record(self):
-        """Get Record object."""
-        if self.recordmetadata:
-            return Record(self.recordmetadata.json, model=self.recordmetadata)
-        else:
-            return None
-
-    @property
-    def deposit_id(self):
-        """Get deposit identifier."""
-        if self.record and '_deposit' in self.record:
-            return self.record['_deposit']['id']
-        else:
-            return None
-
     def __repr__(self):
         """Get release representation."""
-        return ('<Release {self.tag}:{self.release_id} ({self.status.title})>'
-                .format(self=self))
+        return f"<Release {self.tag}:{self.release_id} ({self.status.title})>"
```

### Comparing `invenio-github-1.0.0a9/invenio_github/proxies.py` & `invenio-github-1.0.0b1/invenio_github/proxies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -20,14 +20,11 @@
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Proxy for current previewer."""
 
-from __future__ import absolute_import, print_function
-
 from flask import current_app
 from werkzeug.local import LocalProxy
 
-current_github = LocalProxy(
-    lambda: current_app.extensions['invenio-github'])
+current_github = LocalProxy(lambda: current_app.extensions["invenio-github"])
```

### Comparing `invenio-github-1.0.0a9/invenio_github/version.py` & `invenio-github-1.0.0b1/tests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+#!/usr/bin/env sh
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -18,16 +19,8 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
-"""Version information for Invenio-GitHub.
-
-This file is imported by ``invenio_github.__init__``,
-and parsed by ``setup.py``.
-"""
-
-from __future__ import absolute_import, print_function
-
-__version__ = "1.0.0a9"
+"""Unit test for Invenio-Github."""
```

### Comparing `invenio-github-1.0.0a9/invenio_github.egg-info/PKG-INFO` & `invenio-github-1.0.0b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0a9
-Summary: Invenio module that adds GitHub integration to the platform.
+Version: 1.0.0b1
+Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
-License: GPLv2
+License: MIT
 Description: ..
             This file is part of Invenio.
-            Copyright (C) 2016 CERN.
+            Copyright (C) 2023 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
             License, or (at your option) any later version.
         
             Invenio is distributed in the hope that it will be
@@ -52,18 +52,17 @@
         Invenio module that adds GitHub integration to the platform.
         
         *This is an experimental developer preview release.*
         
         * Free software: GPLv2 license
         * Documentation: https://invenio-github.readthedocs.io/
         
-        
         ..
             This file is part of Invenio.
-            Copyright (C) 2016 CERN.
+            Copyright (C) 2016-2022 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
             License, or (at your option) any later version.
         
             Invenio is distributed in the hope that it will be
@@ -80,26 +79,24 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
-        Version v1.0.0a9 (released 2016-09-29)
+        Version v1.0.0b1 (released 2023-07-03)
+        
+        - Initial beta release.
+        
+        Version v1.0.0a28 (released 2022-10-24)
         
         - Initial public release.
         
 Keywords: invenio github
 Platform: any
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7
+Provides-Extra: docs
+Provides-Extra: tests
+Provides-Extra: elasticsearch7
+Provides-Extra: opensearch1
+Provides-Extra: opensearch2
```

### Comparing `invenio-github-1.0.0a9/invenio_github.egg-info/SOURCES.txt` & `invenio-github-1.0.0b1/invenio_github.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 .dockerignore
 .editorconfig
-.travis-devel-requirements.txt
-.travis-lowest-requirements.txt
-.travis-release-requirements.txt
+.git-blame-ignore-revs
+.lgtm
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
+MAINTAINERS
 MANIFEST.in
 README.rst
 RELEASE-NOTES.rst
 babel.ini
-pytest.ini
+constraints-pypi.txt
+pyproject.toml
 requirements-devel.txt
 run-tests.sh
 setup.cfg
 setup.py
 .tx/config
 docs/Makefile
 docs/api.rst
@@ -26,46 +27,43 @@
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/license.rst
 docs/make.bat
 docs/requirements.txt
 docs/usage.rst
-examples/app.py
 invenio_github/__init__.py
-invenio_github/admin.py
 invenio_github/api.py
-invenio_github/bundles.py
 invenio_github/config.py
 invenio_github/errors.py
 invenio_github/ext.py
 invenio_github/handlers.py
 invenio_github/models.py
 invenio_github/proxies.py
 invenio_github/receivers.py
 invenio_github/tasks.py
 invenio_github/utils.py
-invenio_github/version.py
+invenio_github/webpack.py
 invenio_github.egg-info/PKG-INFO
 invenio_github.egg-info/SOURCES.txt
 invenio_github.egg-info/dependency_links.txt
 invenio_github.egg-info/entry_points.txt
 invenio_github.egg-info/not-zip-safe
 invenio_github.egg-info/requires.txt
 invenio_github.egg-info/top_level.txt
-invenio_github/static/js/github/init.js
-invenio_github/static/js/github/view.js
-invenio_github/static/scss/github/github.scss
-invenio_github/templates/invenio_github/base.html
-invenio_github/templates/invenio_github/helpers.html
-invenio_github/templates/invenio_github/settings/base.html
-invenio_github/templates/invenio_github/settings/helpers.html
-invenio_github/templates/invenio_github/settings/index.html
-invenio_github/templates/invenio_github/settings/index_item.html
-invenio_github/templates/invenio_github/settings/view.html
+invenio_github/assets/semantic-ui/js/invenio_github/init.js
+invenio_github/assets/semantic-ui/js/invenio_github/view.js
+invenio_github/assets/semantic-ui/less/github/github.scss
+invenio_github/templates/semantic-ui/invenio_github/base.html
+invenio_github/templates/semantic-ui/invenio_github/helpers.html
+invenio_github/templates/semantic-ui/invenio_github/settings/base.html
+invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
+invenio_github/templates/semantic-ui/invenio_github/settings/index.html
+invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
+invenio_github/templates/semantic-ui/invenio_github/settings/view.html
 invenio_github/translations/messages.pot
 invenio_github/translations/cs/LC_MESSAGES/messages.po
 invenio_github/translations/da/LC_MESSAGES/messages.po
 invenio_github/translations/de/LC_MESSAGES/messages.po
 invenio_github/translations/en/LC_MESSAGES/messages.mo
 invenio_github/translations/en/LC_MESSAGES/messages.po
 invenio_github/translations/es/LC_MESSAGES/messages.po
@@ -73,13 +71,14 @@
 invenio_github/translations/it/LC_MESSAGES/messages.po
 invenio_github/views/__init__.py
 invenio_github/views/badge.py
 invenio_github/views/github.py
 tests/__init__.py
 tests/conftest.py
 tests/fixtures.py
-tests/helpers.py
+tests/test_api.py
 tests/test_badge.py
 tests/test_invenio_github.py
 tests/test_models.py
 tests/test_tasks.py
+tests/test_views.py
 tests/test_webhook.py
```

### Comparing `invenio-github-1.0.0a9/invenio_github.egg-info/entry_points.txt` & `invenio-github-1.0.0b1/invenio_github.egg-info/entry_points.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-[invenio_admin.views]
-invenio_github_repository = invenio_github.admin:repository_adminview
-invenio_github_requests = invenio_github.admin:release_adminview
+[invenio_assets.webpack]
+invenio_github = invenio_github.webpack:theme
 
-[invenio_assets.bundles]
-invenio_github_css = invenio_github.bundles:css
-invenio_github_js = invenio_github.bundles:js
+[invenio_base.api_apps]
+invenio_github = invenio_github:InvenioGitHub
+
+[invenio_base.api_blueprints]
+invenio_github = invenio_github.views.github:blueprint_api
 
 [invenio_base.apps]
 invenio_github = invenio_github:InvenioGitHub
 
 [invenio_base.blueprints]
 invenio_github_badge = invenio_github.views.badge:blueprint
 invenio_github_github = invenio_github.views.github:blueprint
```

### Comparing `invenio-github-1.0.0a9/tests/test_badge.py` & `invenio-github-1.0.0b1/tests/test_badge.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 
 """Test cases for badge creation."""
 
 from __future__ import absolute_import
 
 from flask import url_for
 
-
-def test_badge_views(app, release_model):
-    """Test create_badge method."""
-    with app.test_client() as client:
-        badge_url = url_for('invenio_github_badge.index',
-                            github_id=release_model.release_id)
-        badge_resp = client.get(badge_url)
-        assert release_model.record['doi'] in badge_resp.location
-
-    with app.test_client() as client:
-        # Test with non-existent github id
-        badge_url = url_for('invenio_github_badge.index', github_id=42)
-        badge_resp = client.get(badge_url)
-        assert badge_resp.status_code == 404
+# TODO uncomment when migrated
+# def test_badge_views(app, release_model):
+#     """Test create_badge method."""
+#     with app.test_client() as client:
+#         badge_url = url_for(
+#             "invenio_github_badge.index", github_id=release_model.release_id
+#         )
+#         badge_resp = client.get(badge_url)
+#         assert release_model.record["doi"] in badge_resp.location
+
+#     with app.test_client() as client:
+#         # Test with non-existent github id
+#         badge_url = url_for("invenio_github_badge.index", github_id=42)
+#         badge_resp = client.get(badge_url)
+#         assert badge_resp.status_code == 404
```

### Comparing `invenio-github-1.0.0a9/tests/test_invenio_github.py` & `invenio-github-1.0.0b1/tests/test_invenio_github.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -21,32 +21,30 @@
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 """Module tests."""
 
-from __future__ import absolute_import, print_function
-
 from flask import Flask
-from flask_babelex import Babel
 
 from invenio_github import InvenioGitHub
 
 
 def test_version():
     """Test version import."""
     from invenio_github import __version__
+
     assert __version__
 
 
 def test_init():
     """Test extension initialization."""
-    app = Flask('testapp')
+    app = Flask("testapp")
     ext = InvenioGitHub(app)
-    assert 'invenio-github' in app.extensions
+    assert "invenio-github" in app.extensions
 
-    app = Flask('testapp')
+    app = Flask("testapp")
     ext = InvenioGitHub()
-    assert 'invenio-github' not in app.extensions
+    assert "invenio-github" not in app.extensions
     ext.init_app(app)
-    assert 'invenio-github' in app.extensions
+    assert "invenio-github" in app.extensions
```

### Comparing `invenio-github-1.0.0a9/tests/test_models.py` & `invenio-github-1.0.0b1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
+# Copyright (C) 2023 Graz University of Technology.
 #
-# Invenio is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# Invenio is free software; you can redistribute it
+# and/or modify it under the terms of the GNU General Public License as
+# published by the Free Software Foundation; either version 2 of the
+# License, or (at your option) any later version.
 #
-# Invenio is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# Invenio is distributed in the hope that it will be
+# useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+# General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with Invenio. If not, see <http://www.gnu.org/licenses/>.
+# along with Invenio; if not, write to the
+# Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
+# MA 02111-1307, USA.
 #
-# In applying this licence, CERN does not waive the privileges and immunities
-# granted to it by virtue of its status as an Intergovernmental Organization
-# or submit itself to any jurisdiction.
+# In applying this license, CERN does not
+# waive the privileges and immunities granted to it by virtue of its status
+# as an Intergovernmental Organization or submit itself to any jurisdiction.
 
-"""Test cases for badge creation."""
+"""Invenio module that adds GitHub integration to the platform."""
 
-from __future__ import absolute_import
+from setuptools import setup
 
-from flask import url_for
-
-from invenio_github.models import Repository
-
-
-def test_repository_unbound(app):
-    """Test create_badge method."""
-    assert Repository(name='org/repo', github_id=1).latest_release() is None
+setup()
```

### Comparing `invenio-github-1.0.0a9/tests/test_tasks.py` & `invenio-github-1.0.0b1/tests/test_webhook.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2014, 2015, 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be useful,
@@ -16,79 +16,89 @@
 # You should have received a copy of the GNU General Public License
 # along with Invenio. If not, see <http://www.gnu.org/licenses/>.
 #
 # In applying this licence, CERN does not waive the privileges and immunities
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
 
-from __future__ import absolute_import
+"""Test GitHub hook."""
 
-from invenio_files_rest.models import Bucket
-from invenio_webhooks.models import Event
-from mock import patch
-
-from invenio_github.api import GitHubRelease
-from invenio_github.models import Release, ReleaseStatus, Repository
-
-from . import fixtures
-
-
-def test_handle_payload(app, db, location, tester_id, remote_token,
-                        github_api):
+import json
 
-    from invenio_webhooks.models import Event
-
-    extra_data = remote_token.remote_account.extra_data
+# from invenio_rdm_records.proxies import current_rdm_records_service
+from invenio_webhooks.models import Event
+from sqlalchemy.orm.exc import NoResultFound
 
-    assert '1' in extra_data['repos']
-    assert 'repo-1' in extra_data['repos']['1']['full_name']
-    assert '2' in extra_data['repos']
-    assert 'repo-2' in extra_data['repos']['2']['full_name']
+from invenio_github.models import ReleaseStatus, Repository
 
-    # Create the repository that will make the release
 
-    with db.session.begin_nested():
-        Repository.enable(tester_id, github_id=1, name='repo-1', hook=1234)
-        event = Event(
-            receiver_id='github',
-            user_id=tester_id,
-            payload=fixtures.PAYLOAD('auser', 'repo-1', 1)
-        )
+def test_webhook_post(app, db, tester_id, remote_token, github_api):
+    """Test webhook POST success."""
+    from . import fixtures
+
+    repo_id = 3
+    repo_name = "arepo"
+    hook = 1234
+    tag = "v1.0"
+
+    # Create a repository
+    repo = Repository.get(github_id=repo_id, name=repo_name)
+    if not repo:
+        repo = Repository.create(tester_id, repo_id, repo_name)
+
+    # Enable repository webhook.
+    Repository.enable(repo, tester_id, hook)
+
+    # JSON payload parsing.
+    payload = json.dumps(fixtures.PAYLOAD("auser", repo_name, repo_id, tag))
+    headers = [("Content-Type", "application/json")]
+    with app.test_request_context(headers=headers, data=payload):
+        event = Event.create(receiver_id="github", user_id=tester_id)
+        # Add event to session. Otherwise defaults are not added (e.g. response and response_code)
         db.session.add(event)
+        db.session.commit()
+        event.process()
 
-    with patch('invenio_deposit.api.Deposit.indexer'):
+    assert event.response_code == 202
+    # Validate that a release was created
+    assert repo.releases.count() == 1
+    release = repo.releases.first()
+    assert release.status == ReleaseStatus.PUBLISHED
+    assert release.release_id == event.payload["release"]["id"]
+    assert release.tag == tag
+    # This uuid is a fake one set by TestGithubRelease fixture
+    assert str(release.record_id) == "445aaacd-9de1-41ab-af52-25ab6cb93df7"
+    assert release.errors is None
+
+
+def test_webhook_post_fail(app, tester_id, remote_token, github_api):
+    """Test webhook POST failure."""
+    from . import fixtures
+
+    repo_id = 3
+    repo_name = "arepo"
+    hook = 1234
+
+    # Create a repository
+    repo = Repository.get(github_id=repo_id, name=repo_name)
+    if not repo:
+        repo = Repository.create(tester_id, repo_id, repo_name)
+
+    # Enable repository webhook.
+    Repository.enable(repo, tester_id, hook)
+
+    # Create an invalid payload (fake repo)
+    fake_payload = json.dumps(
+        fixtures.PAYLOAD("fake_user", "fake_repo", 1000, "v1000.0")
+    )
+    headers = [("Content-Type", "application/json")]
+    with app.test_request_context(headers=headers, data=fake_payload):
+        # user_id = request.oauth.access_token.user_id
+        event = Event.create(receiver_id="github", user_id=tester_id)
         event.process()
 
-        repo_1 = Repository.query.filter_by(name='repo-1', github_id=1).first()
-        assert repo_1.releases.count() == 1
+    # Repo does not exist
+    assert event.response_code == 404
 
-        release = repo_1.releases.first()
-        assert release.status == ReleaseStatus.PUBLISHED
-        assert release.errors is None
-        assert release.tag == 'v1.0'
-        assert release.record is not None
-        assert release.record.get('control_number') == '1'
-        record_files = release.record.get('_files')
-        assert len(record_files) == 1
-        assert record_files[0]['size'] > 0
-
-        bucket = Bucket.get(record_files[0]['bucket'])
-        assert bucket is not None
-        assert len(bucket.objects) == 1
-        assert bucket.objects[0].key == 'auser/repo-1-v1.0.zip'
-
-
-def test_extract_metadata(app, db, tester_id, remote_token, github_api):
-
-    Repository.enable(tester_id, github_id=2, name='repo-2', hook=1234)
-    event = Event(
-        receiver_id='github',
-        user_id=tester_id,
-        payload=fixtures.PAYLOAD('auser', 'repo-2', 2, tag='v1.0'),
-    )
-    release = Release.create(event)
-    gh = GitHubRelease(release)
-    metadata = gh.metadata
-
-    assert metadata['upload_type'] == 'dataset'
-    assert metadata['license'] == 'mit-license'
-    assert len(metadata['creators']) == 2
+    # Create an invalid payload (fake user)
+    # TODO 'fake_user' does not match the invenio user 'extra_data'. Should this fail?
+    # TODO what should happen if an event is received and the account is not synced?
```

### Comparing `invenio-github-1.0.0a9/.editorconfig` & `invenio-github-1.0.0b1/.editorconfig`

 * *Files 16% similar despite different names*

```diff
@@ -28,22 +28,14 @@
 [*]
 indent_style = space
 end_of_line = lf
 insert_final_newline = true
 trim_trailing_whitespace = true
 charset = utf-8
 
-# Python files
-[*.py]
-indent_size = 4
-# isort plugin configuration
-known_first_party = invenio_github
-multi_line_output = 2
-default_section = THIRDPARTY
-
 # RST files (used by sphinx)
 [*.rst]
 indent_size = 4
 
 # CSS, HTML, JS, JSON, YML
 [*.{css,html,js,json,yml}]
 indent_size = 2
```

### Comparing `invenio-github-1.0.0a9/AUTHORS.rst` & `invenio-github-1.0.0b1/AUTHORS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -26,11 +26,12 @@
 =======
 
 Invenio module that adds GitHub integration to the platform.
 
 - Adrian Pawel Baran <adrian.pawel.baran@cern.ch>
 - Alexander Ioannidis <a.ioannidis@cern.ch>
 - Amit Kapadia <akapad@gmail.com>
+- Charlie Lewis <clewis@iqt.org>
 - Dan Blanchard <dan.blanchard@gmail.com>
 - Jiri Kuncar <jiri.kuncar@cern.ch>
 - Lars Holm Nielsen <lars.holm.nielsen@cern.ch>
 - Tibor Simko <tibor.simko@cern.ch>
```

### Comparing `invenio-github-1.0.0a9/CHANGES.rst` & `invenio-github-1.0.0b1/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ..
     This file is part of Invenio.
-    Copyright (C) 2016 CERN.
+    Copyright (C) 2016-2022 CERN.
 
     Invenio is free software; you can redistribute it
     and/or modify it under the terms of the GNU General Public License as
     published by the Free Software Foundation; either version 2 of the
     License, or (at your option) any later version.
 
     Invenio is distributed in the hope that it will be
@@ -21,10 +21,14 @@
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 Changes
 =======
 
-Version v1.0.0a9 (released 2016-09-29)
+Version v1.0.0b1 (released 2023-07-03)
+
+- Initial beta release.
+
+Version v1.0.0a28 (released 2022-10-24)
 
 - Initial public release.
```

### Comparing `invenio-github-1.0.0a9/CONTRIBUTING.rst` & `invenio-github-1.0.0b1/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -91,16 +91,16 @@
    documentation and run doctests.
 
 6. Commit your changes and push your branch to GitHub:
 
    .. code-block:: console
 
       $ git add .
-      $ git commit -s 
-          -m "component: title without verbs" 
+      $ git commit -s
+          -m "component: title without verbs"
           -m "* NEW Adds your new feature."
           -m "* FIX Fixes an existing issue."
           -m "* BETTER Improves and existing feature."
           -m "* Changes something that should not be visible in release notes"
       $ git push origin name-of-your-bugfix-or-feature
 
 7. Submit a pull request through the GitHub website.
```

### Comparing `invenio-github-1.0.0a9/MANIFEST.in` & `invenio-github-1.0.0b1/MANIFEST.in`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016 CERN.
+# Copyright (C) 2023 CERN.
 #
 # Invenio is free software; you can redistribute it
 # and/or modify it under the terms of the GNU General Public License as
 # published by the Free Software Foundation; either version 2 of the
 # License, or (at your option) any later version.
 #
 # Invenio is distributed in the hope that it will be
@@ -25,15 +25,17 @@
 
 include *.rst
 include *.sh
 include *.txt
 include .dockerignore
 include .editorconfig
 include .tx/config
+include .lgtm
 include LICENSE
+include MAINTAINERS
 include babel.ini
 include docs/requirements.txt
 include pytest.ini
 recursive-include docs *.bat
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs Makefile
@@ -41,7 +43,9 @@
 recursive-include invenio_github *.css
 recursive-include invenio_github *.html
 recursive-include invenio_github *.js
 recursive-include invenio_github *.png
 recursive-include invenio_github *.po *.pot *.mo
 recursive-include invenio_github *.scss
 recursive-include invenio_github *.ttf
+recursive-include tests *.py
+include .git-blame-ignore-revs
```

### Comparing `invenio-github-1.0.0a9/README.rst` & `invenio-github-1.0.0b1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ..
     This file is part of Invenio.
-    Copyright (C) 2016 CERN.
+    Copyright (C) 2023 CERN.
 
     Invenio is free software; you can redistribute it
     and/or modify it under the terms of the GNU General Public License as
     published by the Free Software Foundation; either version 2 of the
     License, or (at your option) any later version.
 
     Invenio is distributed in the hope that it will be
```

### Comparing `invenio-github-1.0.0a9/RELEASE-NOTES.rst` & `invenio-github-1.0.0b1/RELEASE-NOTES.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-=========================
- Invenio-GitHub v1.0.0a9
-=========================
+==========================
+ Invenio-GitHub v1.0.0a28
+==========================
 
-Invenio-GitHub v1.0.0a9 was released on September 29, 2016.
+Invenio-GitHub v1.0.0a28 was released on October 24, 2022.
 
 About
 -----
 
 Invenio module that adds GitHub integration to the platform.
 
 *This is an experimental developer preview release.*
@@ -15,15 +15,15 @@
 ----------
 
 - Initial public release.
 
 Installation
 ------------
 
-   $ pip install invenio-github==v1.0.0a9
+   $ pip install invenio-github==v1.0.0a28
 
 Documentation
 -------------
 
    http://invenio-github.readthedocs.io/
 
 Happy hacking and thanks for flying Invenio-GitHub.
```

### Comparing `invenio-github-1.0.0a9/babel.ini` & `invenio-github-1.0.0b1/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0a9/pytest.ini` & `invenio-github-1.0.0b1/requirements-devel.txt`

 * *Files 27% similar despite different names*

```diff
@@ -17,10 +17,7 @@
 # along with Invenio; if not, write to the
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
 # MA 02111-1307, USA.
 #
 # In applying this license, CERN does not
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
-
-[pytest]
-addopts = --pep8 --ignore=docs --cov=invenio_github --cov-report=term-missing
```

### Comparing `invenio-github-1.0.0a9/PKG-INFO` & `invenio-github-1.0.0b1/invenio_github.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0a9
-Summary: Invenio module that adds GitHub integration to the platform.
+Version: 1.0.0b1
+Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
-License: GPLv2
+License: MIT
 Description: ..
             This file is part of Invenio.
-            Copyright (C) 2016 CERN.
+            Copyright (C) 2023 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
             License, or (at your option) any later version.
         
             Invenio is distributed in the hope that it will be
@@ -52,18 +52,17 @@
         Invenio module that adds GitHub integration to the platform.
         
         *This is an experimental developer preview release.*
         
         * Free software: GPLv2 license
         * Documentation: https://invenio-github.readthedocs.io/
         
-        
         ..
             This file is part of Invenio.
-            Copyright (C) 2016 CERN.
+            Copyright (C) 2016-2022 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
             License, or (at your option) any later version.
         
             Invenio is distributed in the hope that it will be
@@ -80,26 +79,24 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
-        Version v1.0.0a9 (released 2016-09-29)
+        Version v1.0.0b1 (released 2023-07-03)
+        
+        - Initial beta release.
+        
+        Version v1.0.0a28 (released 2022-10-24)
         
         - Initial public release.
         
 Keywords: invenio github
 Platform: any
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7
+Provides-Extra: docs
+Provides-Extra: tests
+Provides-Extra: elasticsearch7
+Provides-Extra: opensearch1
+Provides-Extra: opensearch2
```

