# Comparing `tmp/invenio-webhooks-1.0.0a3.tar.gz` & `tmp/invenio-webhooks-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-webhooks-1.0.0a3.tar", last modified: Tue Aug  2 14:39:00 2016, max compression
+gzip compressed data, was "dist/invenio-webhooks-1.0.0a4.tar", last modified: Mon Oct  3 14:28:04 2016, max compression
```

## Comparing `invenio-webhooks-1.0.0a3.tar` & `invenio-webhooks-1.0.0a4.tar`

### file list

```diff
@@ -1,77 +1,82 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/.tx/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1796 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/.tx/config
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/docs/
--rw-rw-r--   0 travis    (1000) travis    (1000)     7449 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/Makefile
--rw-rw-r--   0 travis    (1000) travis    (1000)     1412 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/api.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/authors.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/changes.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)    10675 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/conf.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1013 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/contributing.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1569 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/index.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/installation.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)      867 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/license.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     7001 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/make.bat
--rw-rw-r--   0 travis    (1000) travis    (1000)     1026 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/docs/usage.rst
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/examples/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1409 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/examples/app.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/de/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/de/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      462 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/de/LC_MESSAGES/messages.mo
--rw-rw-r--   0 travis    (1000) travis    (1000)      668 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/de/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/es/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/es/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      462 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/es/LC_MESSAGES/messages.mo
--rw-rw-r--   0 travis    (1000) travis    (1000)      669 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/es/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/fr/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/fr/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      461 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/fr/LC_MESSAGES/messages.mo
--rw-rw-r--   0 travis    (1000) travis    (1000)      667 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/fr/LC_MESSAGES/messages.po
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/it/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/it/LC_MESSAGES/
--rw-rw-r--   0 travis    (1000) travis    (1000)      462 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/it/LC_MESSAGES/messages.mo
--rw-rw-r--   0 travis    (1000) travis    (1000)      669 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/it/LC_MESSAGES/messages.po
--rw-rw-r--   0 travis    (1000) travis    (1000)      639 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/translations/messages.pot
--rw-rw-r--   0 travis    (1000) travis    (1000)     1311 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1192 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/config.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2882 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/ext.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7631 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/models.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1170 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/proxies.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1941 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/signatures.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1193 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/version.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3397 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/invenio_webhooks/views.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)     4842 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)     1598 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      369 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-08-02 14:38:34.000000 invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (1000) travis    (1000)      677 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/requires.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       17 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/tests/
--rw-rw-r--   0 travis    (1000) travis    (1000)     4797 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/tests/conftest.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     6196 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/tests/test_api.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1975 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/tests/test_invenio_webhooks.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5788 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/tests/test_receivers.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      124 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/.dockerignore
--rw-rw-r--   0 travis    (1000) travis    (1000)     1588 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/.editorconfig
--rw-rw-r--   0 travis    (1000) travis    (1000)       91 2016-08-02 14:38:26.000000 invenio-webhooks-1.0.0a3/.travis-devel-requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       91 2016-08-02 14:38:25.000000 invenio-webhooks-1.0.0a3/.travis-lowest-requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       91 2016-08-02 14:38:25.000000 invenio-webhooks-1.0.0a3/.travis-release-requirements.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)     1297 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/AUTHORS.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1136 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/CHANGES.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     3482 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)       26 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/INSTALL.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)    18092 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/LICENSE
--rw-rw-r--   0 travis    (1000) travis    (1000)     1639 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/MANIFEST.in
--rw-rw-r--   0 travis    (1000) travis    (1000)     1999 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/README.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)      770 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/RELEASE-NOTES.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     1289 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/babel.ini
--rw-rw-r--   0 travis    (1000) travis    (1000)     1061 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/pytest.ini
--rw-rw-r--   0 travis    (1000) travis    (1000)     1245 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/requirements-devel.txt
--rwxrwxr-x   0 travis    (1000) travis    (1000)     1222 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/run-tests.sh
--rw-rw-r--   0 travis    (1000) travis    (1000)      674 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/setup.cfg
--rw-rw-r--   0 travis    (1000) travis    (1000)     3998 2016-08-02 14:38:11.000000 invenio-webhooks-1.0.0a3/setup.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4842 2016-08-02 14:39:00.000000 invenio-webhooks-1.0.0a3/PKG-INFO
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/.tx/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1801 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/.tx/config
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/docs/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7449 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/Makefile
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1412 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/api.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/authors.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/changes.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)    10729 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/conf.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1013 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/contributing.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1573 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/index.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/installation.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)      867 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/license.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7001 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/make.bat
+-rw-rw-r--   0 travis    (1000) travis    (1000)       17 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/requirements.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1026 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/docs/usage.rst
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/examples/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1409 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/examples/app.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/cs/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/cs/LC_MESSAGES/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      829 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/cs/LC_MESSAGES/messages.po
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/da/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/da/LC_MESSAGES/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      803 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/da/LC_MESSAGES/messages.po
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/de/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/de/LC_MESSAGES/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      803 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/de/LC_MESSAGES/messages.po
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/es/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/es/LC_MESSAGES/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      804 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/es/LC_MESSAGES/messages.po
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/fr/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/fr/LC_MESSAGES/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      912 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/fr/LC_MESSAGES/messages.po
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/it/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/it/LC_MESSAGES/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      910 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/it/LC_MESSAGES/messages.po
+-rw-rw-r--   0 travis    (1000) travis    (1000)      740 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/translations/messages.pot
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1311 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1192 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/config.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2882 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/ext.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7631 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/models.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1170 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/proxies.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1941 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/signatures.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1193 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/version.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3397 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/invenio_webhooks/views.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4818 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1524 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)      369 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-10-03 14:27:32.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (1000) travis    (1000)      692 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/requires.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)       17 2016-10-03 14:28:03.000000 invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/tests/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4748 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/tests/conftest.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     6196 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/tests/test_api.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1975 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/tests/test_invenio_webhooks.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5788 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/tests/test_receivers.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      124 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/.dockerignore
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1588 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/.editorconfig
+-rw-rw-r--   0 travis    (1000) travis    (1000)       60 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/.lgtm
+-rw-rw-r--   0 travis    (1000) travis    (1000)      106 2016-10-03 14:27:22.000000 invenio-webhooks-1.0.0a4/.travis-devel-requirements.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)      106 2016-10-03 14:27:22.000000 invenio-webhooks-1.0.0a4/.travis-lowest-requirements.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)      106 2016-10-03 14:27:22.000000 invenio-webhooks-1.0.0a4/.travis-release-requirements.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1335 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/AUTHORS.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1142 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/CHANGES.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3482 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)       26 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/INSTALL.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)    18092 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/LICENSE
+-rw-rw-r--   0 travis    (1000) travis    (1000)      106 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/MAINTAINERS
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1703 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/MANIFEST.in
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1997 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/README.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)      771 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/RELEASE-NOTES.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1289 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/babel.ini
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1061 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/pytest.ini
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1245 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/requirements-devel.txt
+-rwxrwxr-x   0 travis    (1000) travis    (1000)     1222 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/run-tests.sh
+-rw-rw-r--   0 travis    (1000) travis    (1000)      674 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/setup.cfg
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3937 2016-10-03 14:27:06.000000 invenio-webhooks-1.0.0a4/setup.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4818 2016-10-03 14:28:04.000000 invenio-webhooks-1.0.0a4/PKG-INFO
```

### Comparing `invenio-webhooks-1.0.0a3/.tx/config` & `invenio-webhooks-1.0.0a4/.tx/config`

 * *Files 2% similar despite different names*

```diff
@@ -39,12 +39,12 @@
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
 host = https://www.transifex.com
 
-[invenio-webhooks.messagespot]
+[invenio.invenio-webhooks-messages]
 file_filter = invenio_webhooks/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_webhooks/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-webhooks-1.0.0a3/docs/Makefile` & `invenio-webhooks-1.0.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/docs/api.rst` & `invenio-webhooks-1.0.0a4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/docs/authors.rst` & `invenio-webhooks-1.0.0a4/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/docs/changes.rst` & `invenio-webhooks-1.0.0a4/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/docs/conf.py` & `invenio-webhooks-1.0.0a4/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,16 +133,16 @@
     'description': 'Invenio module for processing webhook events.',
     'github_user': 'inveniosoftware',
     'github_repo': 'invenio-webhooks',
     'github_button': False,
     'github_banner': True,
     'show_powered_by': False,
     'extra_nav_links': {
-        'invenio-webhooks@GitHub': 'http://github.com/inveniosoftware/invenio-webhooks',
-        'invenio-webhooks@PyPI': 'http://pypi.python.org/pypi/invenio-webhooks/',
+        'invenio-webhooks@GitHub': 'https://github.com/inveniosoftware/invenio-webhooks',
+        'invenio-webhooks@PyPI': 'https://pypi.python.org/pypi/invenio-webhooks/',
     }
 }
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 # Theme options are theme-specific and customize the look and feel of a theme
@@ -325,7 +325,10 @@
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {'https://docs.python.org/': None}
+
+# Autodoc configuraton.
+autoclass_content = 'both'
```

### Comparing `invenio-webhooks-1.0.0a3/docs/contributing.rst` & `invenio-webhooks-1.0.0a4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/docs/index.rst` & `invenio-webhooks-1.0.0a4/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 .. include:: ../README.rst
 
 User's Guide
 ------------
 
 This part of the documentation will show you how to get started in using
-Invenio-Base.
+Invenio-Webhooks.
 
 .. toctree::
    :maxdepth: 2
 
    installation
    usage
```

### Comparing `invenio-webhooks-1.0.0a3/docs/installation.rst` & `invenio-webhooks-1.0.0a4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/docs/license.rst` & `invenio-webhooks-1.0.0a4/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/docs/make.bat` & `invenio-webhooks-1.0.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/docs/usage.rst` & `invenio-webhooks-1.0.0a4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/examples/app.py` & `invenio-webhooks-1.0.0a4/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks/translations/fr/LC_MESSAGES/messages.po` & `invenio-webhooks-1.0.0a4/invenio_webhooks/translations/da/LC_MESSAGES/messages.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-# French translations for invenio-webhooks.
-# Copyright (C) 2015 ORGANIZATION
+# Translations template for invenio-webhooks.
+# Copyright (C) 2016 CERN
 # This file is distributed under the same license as the invenio-webhooks
 # project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2015.
-#
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
+# 
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-webhooks 0.1.0.dev20150000\n"
-"Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2015-08-04 21:08+0200\n"
-"PO-Revision-Date: 2015-08-04 21:08+0200\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: fr <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n > 1)\n"
+"Project-Id-Version: invenio-webhooks 1.0.0a4.dev20160802\n"
+"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
+"POT-Creation-Date: 2016-08-19 15:19+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.0\n"
+"Generated-By: Babel 2.3.4\n"
+"Language: da\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+#: invenio_webhooks/views.py:50
+msgid "Allow notifications from external service."
+msgstr ""
```

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks/__init__.py` & `invenio-webhooks-1.0.0a4/invenio_webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks/config.py` & `invenio-webhooks-1.0.0a4/invenio_webhooks/config.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks/ext.py` & `invenio-webhooks-1.0.0a4/invenio_webhooks/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks/models.py` & `invenio-webhooks-1.0.0a4/invenio_webhooks/models.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks/proxies.py` & `invenio-webhooks-1.0.0a4/invenio_webhooks/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks/signatures.py` & `invenio-webhooks-1.0.0a4/invenio_webhooks/signatures.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks/version.py` & `invenio-webhooks-1.0.0a4/invenio_webhooks/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
 This file is imported by ``invenio_webhooks.__init__``,
 and parsed by ``setup.py``.
 """
 
 from __future__ import absolute_import, print_function
 
-__version__ = "1.0.0a3"
+__version__ = "1.0.0a4"
```

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks/views.py` & `invenio-webhooks-1.0.0a4/invenio_webhooks/views.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/PKG-INFO` & `invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: invenio-webhooks
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Invenio module for processing webhook events.
 Home-page: https://github.com/inveniosoftware/invenio-webhooks
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: GPLv2
 Description: ..
             This file is part of Invenio.
@@ -50,20 +50,20 @@
         
         
         Invenio module for processing webhook events.
         
         *This is an experimental developer preview release.*
         
         * Free software: GPLv2 license
-        * Documentation: https://pythonhosted.org/invenio-webhooks/
+        * Documentation: https://invenio-webhooks.readthedocs.io/
         
         
         ..
             This file is part of Invenio.
-            Copyright (C) 2015 CERN.
+            Copyright (C) 2015, 2016 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
             License, or (at your option) any later version.
         
             Invenio is distributed in the hope that it will be
@@ -79,15 +79,15 @@
             In applying this license, CERN does not
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         Changes
         =======
         
-        Version 1.0.0a3 (release 2016-08-02)
+        Version 1.0.0a4 (release 2016-10-03)
         
         - Port to new structure for Invenio 3.
         
         Version 0.1.0 (release 2015-08-05)
         
         - Initial public release.
         
@@ -99,11 +99,10 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 1 - Planning
```

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/SOURCES.txt` & `invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 .dockerignore
 .editorconfig
+.lgtm
 .travis-devel-requirements.txt
 .travis-lowest-requirements.txt
 .travis-release-requirements.txt
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
 pytest.ini
 requirements-devel.txt
 run-tests.sh
@@ -24,14 +26,15 @@
 docs/changes.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/license.rst
 docs/make.bat
+docs/requirements.txt
 docs/usage.rst
 examples/app.py
 invenio_webhooks/__init__.py
 invenio_webhooks/config.py
 invenio_webhooks/ext.py
 invenio_webhooks/models.py
 invenio_webhooks/proxies.py
@@ -42,19 +45,17 @@
 invenio_webhooks.egg-info/SOURCES.txt
 invenio_webhooks.egg-info/dependency_links.txt
 invenio_webhooks.egg-info/entry_points.txt
 invenio_webhooks.egg-info/not-zip-safe
 invenio_webhooks.egg-info/requires.txt
 invenio_webhooks.egg-info/top_level.txt
 invenio_webhooks/translations/messages.pot
-invenio_webhooks/translations/de/LC_MESSAGES/messages.mo
+invenio_webhooks/translations/cs/LC_MESSAGES/messages.po
+invenio_webhooks/translations/da/LC_MESSAGES/messages.po
 invenio_webhooks/translations/de/LC_MESSAGES/messages.po
-invenio_webhooks/translations/es/LC_MESSAGES/messages.mo
 invenio_webhooks/translations/es/LC_MESSAGES/messages.po
-invenio_webhooks/translations/fr/LC_MESSAGES/messages.mo
 invenio_webhooks/translations/fr/LC_MESSAGES/messages.po
-invenio_webhooks/translations/it/LC_MESSAGES/messages.mo
 invenio_webhooks/translations/it/LC_MESSAGES/messages.po
 tests/conftest.py
 tests/test_api.py
 tests/test_invenio_webhooks.py
 tests/test_receivers.py
```

### Comparing `invenio-webhooks-1.0.0a3/invenio_webhooks.egg-info/requires.txt` & `invenio-webhooks-1.0.0a4/invenio_webhooks.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Flask-BabelEx>=0.9.2
+Flask>=0.11.1
 cryptography>=1.3.1
-invenio-db>=1.0.0a9
-invenio-oauth2server>=1.0.0a1
+invenio-db>=1.0.0b1
+invenio-oauth2server>=1.0.0a10
 
 [all]
 celery>=3.0
 Sphinx>=1.4.2
 Flask-CeleryExt>=0.1.0
 check-manifest>=0.25
 coverage>=4.0
```

### Comparing `invenio-webhooks-1.0.0a3/tests/conftest.py` & `invenio-webhooks-1.0.0a4/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 import os
 
 import pytest
 from flask import Flask
 from flask_babelex import Babel
 from flask_breadcrumbs import Breadcrumbs
 from flask_celeryext import FlaskCeleryExt
-from flask_cli import FlaskCLI
 from flask_mail import Mail
 from flask_menu import Menu
 from invenio_accounts import InvenioAccounts
 from invenio_accounts.views import blueprint as accounts_blueprint
 from invenio_db import InvenioDB, db
 from invenio_oauth2server import InvenioOAuth2Server
 from invenio_oauth2server.models import Token
@@ -67,15 +66,14 @@
         WTF_CSRF_ENABLED=False,
         OAUTHLIB_INSECURE_TRANSPORT=True,
         OAUTH2_CACHE_TYPE='simple',
         SECURITY_PASSWORD_HASH='plaintext',
         SECURITY_PASSWORD_SCHEMES=['plaintext'],
         SECURITY_DEPRECATED_PASSWORD_SCHEMES=[],
     )
-    FlaskCLI(app)
     celeryext = FlaskCeleryExt(app)
     celeryext.celery.flask_app = app  # Make sure both apps are the same!
     Babel(app)
     Mail(app)
     Menu(app)
     Breadcrumbs(app)
     InvenioDB(app)
```

### Comparing `invenio-webhooks-1.0.0a3/tests/test_api.py` & `invenio-webhooks-1.0.0a4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/tests/test_invenio_webhooks.py` & `invenio-webhooks-1.0.0a4/tests/test_invenio_webhooks.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/tests/test_receivers.py` & `invenio-webhooks-1.0.0a4/tests/test_receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/.editorconfig` & `invenio-webhooks-1.0.0a4/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/AUTHORS.rst` & `invenio-webhooks-1.0.0a4/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ..
     This file is part of Invenio.
-    Copyright (C) 2015 CERN.
+    Copyright (C) 2015, 2016 CERN.
 
     Invenio is free software; you can redistribute it
     and/or modify it under the terms of the GNU General Public License as
     published by the Free Software Foundation; either version 2 of the
     License, or (at your option) any later version.
 
     Invenio is distributed in the hope that it will be
@@ -17,18 +17,17 @@
     Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston,
     MA 02111-1307, USA.
 
     In applying this license, CERN does not
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
-Authors
+Changes
 =======
 
-Invenio module for processing webhook events.
+Version 1.0.0a4 (release 2016-10-03)
 
-- Grzegorz Szpura <grzegorz.szpura@cern.ch>
-- Jiri Kuncar <jiri.kuncar@cern.ch>
-- Konstantinos Kostis <konstantinos.kostis@cern.ch>
-- Lars Holm Nielsen <lars.holm.nielsen@cern.ch>
-- Leonardo Rossi <leonardo.r@cern.ch>
-- Tibor Simko <tibor.simko@cern.ch>
+- Port to new structure for Invenio 3.
+
+Version 0.1.0 (release 2015-08-05)
+
+- Initial public release.
```

### Comparing `invenio-webhooks-1.0.0a3/CONTRIBUTING.rst` & `invenio-webhooks-1.0.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/LICENSE` & `invenio-webhooks-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/MANIFEST.in` & `invenio-webhooks-1.0.0a4/MANIFEST.in`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,19 @@
 include .tx/config
 recursive-include invenio_webhooks *.po *.pot *.mo
 
 # added by check_manifest.py
 include *.rst
 include *.sh
 include *.txt
+include .lgtm
 include LICENSE
+include MAINTAINERS
 include babel.ini
+include docs/requirements.txt
 include pytest.ini
 recursive-include docs *.bat
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs Makefile
 recursive-include examples *.py
 recursive-include invenio_webhooks *.html
```

### Comparing `invenio-webhooks-1.0.0a3/README.rst` & `invenio-webhooks-1.0.0a4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 
 
 Invenio module for processing webhook events.
 
 *This is an experimental developer preview release.*
 
 * Free software: GPLv2 license
-* Documentation: https://pythonhosted.org/invenio-webhooks/
+* Documentation: https://invenio-webhooks.readthedocs.io/
```

### Comparing `invenio-webhooks-1.0.0a3/RELEASE-NOTES.rst` & `invenio-webhooks-1.0.0a4/RELEASE-NOTES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===========================
- Invenio-Webhooks v1.0.0a3
+ Invenio-Webhooks v1.0.0a4
 ===========================
 
-Invenio-Webhooks v1.0.0a3 was released on August 2, 2016.
+Invenio-Webhooks v1.0.0a4 was released on October 3, 2016.
 
 About
 -----
 
 Invenio module for processing webhook events.
 
 *This is an experimental developer preview release.*
@@ -15,22 +15,22 @@
 ----------
 
 - Port to new structure for Invenio 3.
 
 Installation
 ------------
 
-   $ pip install invenio-webhooks==1.0.0a3
+   $ pip install invenio-webhooks==1.0.0a4
 
 Documentation
 -------------
 
-   http://pythonhosted.org/invenio-webhooks/
+   https://invenio-webhooks.readthedocs.io/
 
 Happy hacking and thanks for flying Invenio-Webhooks.
 
 | Invenio Development Team
 |   Email: info@inveniosoftware.org
 |   IRC: #invenio on irc.freenode.net
-|   Twitter: http://twitter.com/inveniosoftware
+|   Twitter: https://twitter.com/inveniosoftware
 |   GitHub: https://github.com/inveniosoftware/invenio-webhooks
 |   URL: http://inveniosoftware.org
```

### Comparing `invenio-webhooks-1.0.0a3/babel.ini` & `invenio-webhooks-1.0.0a4/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/pytest.ini` & `invenio-webhooks-1.0.0a4/pytest.ini`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/requirements-devel.txt` & `invenio-webhooks-1.0.0a4/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/run-tests.sh` & `invenio-webhooks-1.0.0a4/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/setup.cfg` & `invenio-webhooks-1.0.0a4/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-webhooks-1.0.0a3/setup.py` & `invenio-webhooks-1.0.0a4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module for processing webhook events."""
 
 import os
 
 from setuptools import find_packages, setup
-from setuptools.command.test import test as TestCommand
 
 readme = open('README.rst').read()
 history = open('CHANGES.rst').read()
 
 tests_require = [
     'Flask-CeleryExt>=0.1.0',
     'check-manifest>=0.25',
@@ -61,17 +60,18 @@
 setup_requires = [
     'Babel>=1.3',
     'pytest-runner>=2.6.2',
 ]
 
 install_requires = [
     'Flask-BabelEx>=0.9.2',
+    'Flask>=0.11.1',
     'cryptography>=1.3.1',
-    'invenio-db>=1.0.0a9',
-    'invenio-oauth2server>=1.0.0a1',
+    'invenio-db>=1.0.0b1',
+    'invenio-oauth2server>=1.0.0a10',
 ]
 
 packages = find_packages()
 
 
 # Get the version string. Cannot be done with import!
 g = {}
@@ -121,13 +121,12 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: Implementation :: CPython',
         'Development Status :: 1 - Planning',
     ],
 )
```

### Comparing `invenio-webhooks-1.0.0a3/PKG-INFO` & `invenio-webhooks-1.0.0a4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: invenio-webhooks
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Invenio module for processing webhook events.
 Home-page: https://github.com/inveniosoftware/invenio-webhooks
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: GPLv2
 Description: ..
             This file is part of Invenio.
@@ -50,20 +50,20 @@
         
         
         Invenio module for processing webhook events.
         
         *This is an experimental developer preview release.*
         
         * Free software: GPLv2 license
-        * Documentation: https://pythonhosted.org/invenio-webhooks/
+        * Documentation: https://invenio-webhooks.readthedocs.io/
         
         
         ..
             This file is part of Invenio.
-            Copyright (C) 2015 CERN.
+            Copyright (C) 2015, 2016 CERN.
         
             Invenio is free software; you can redistribute it
             and/or modify it under the terms of the GNU General Public License as
             published by the Free Software Foundation; either version 2 of the
             License, or (at your option) any later version.
         
             Invenio is distributed in the hope that it will be
@@ -79,15 +79,15 @@
             In applying this license, CERN does not
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         Changes
         =======
         
-        Version 1.0.0a3 (release 2016-08-02)
+        Version 1.0.0a4 (release 2016-10-03)
         
         - Port to new structure for Invenio 3.
         
         Version 0.1.0 (release 2015-08-05)
         
         - Initial public release.
         
@@ -99,11 +99,10 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 1 - Planning
```

