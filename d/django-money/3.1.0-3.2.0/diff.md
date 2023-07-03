# Comparing `tmp/django-money-3.1.0.tar.gz` & `tmp/django-money-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-money-3.1.0.tar", last modified: Sun Apr 23 20:53:17 2023, max compression
+gzip compressed data, was "django-money-3.2.0.tar", last modified: Mon Jul  3 14:50:17 2023, max compression
```

## Comparing `django-money-3.1.0.tar` & `django-money-3.2.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-23 20:53:09.000000 django-money-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 20:53:09.000000 django-money-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16751 2023-04-23 20:53:17.332533 django-money-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-04-23 20:53:09.000000 django-money-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/django_money.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16751 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 20:53:17.000000 django-money-3.1.0/django_money.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/djmoney/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/djmoney/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/djmoney/contrib/django_rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/django_rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/django_rest_framework/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.328533 django-money-3.1.0/djmoney/contrib/exchange/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/contrib/exchange/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/backends/fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/backends/openexchangerates.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/contrib/exchange/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/contrib/exchange/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/commands/clear_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/management/commands/update_rates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/contrib/exchange/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/contrib/exchange/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/forms/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/models/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/models/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/models/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/money.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/djmoney/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/templatetags/djmoney.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-23 20:53:09.000000 django-money-3.1.0/djmoney/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-23 20:53:09.000000 django-money-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-23 20:53:17.332533 django-money-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-23 20:53:09.000000 django-money-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:53:17.332533 django-money-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39496 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_money.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_reversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-23 20:53:09.000000 django-money-3.1.0/tests/test_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.239062 django-money-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-03 14:50:08.000000 django-money-3.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-03 14:50:08.000000 django-money-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16751 2023-07-03 14:50:17.239062 django-money-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-07-03 14:50:08.000000 django-money-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.231062 django-money-3.2.0/django_money.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16751 2023-07-03 14:50:17.000000 django-money-3.2.0/django_money.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-03 14:50:17.000000 django-money-3.2.0/django_money.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:50:17.000000 django-money-3.2.0/django_money.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-03 14:50:17.000000 django-money-3.2.0/django_money.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 14:50:17.000000 django-money-3.2.0/django_money.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.235062 django-money-3.2.0/djmoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.235062 django-money-3.2.0/djmoney/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.235062 django-money-3.2.0/djmoney/contrib/django_rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/django_rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/django_rest_framework/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.235062 django-money-3.2.0/djmoney/contrib/exchange/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.235062 django-money-3.2.0/djmoney/contrib/exchange/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/backends/fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/backends/openexchangerates.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.235062 django-money-3.2.0/djmoney/contrib/exchange/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/management/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.235062 django-money-3.2.0/djmoney/contrib/exchange/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/management/commands/clear_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/management/commands/update_rates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.239062 django-money-3.2.0/djmoney/contrib/exchange/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/contrib/exchange/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.239062 django-money-3.2.0/djmoney/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.239062 django-money-3.2.0/djmoney/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/models/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/models/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/money.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.239062 django-money-3.2.0/djmoney/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/templatetags/djmoney.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 14:50:08.000000 django-money-3.2.0/djmoney/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-03 14:50:08.000000 django-money-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 14:50:17.239062 django-money-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-03 14:50:08.000000 django-money-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:50:17.239062 django-money-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-03 14:50:08.000000 django-money-3.2.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-07-03 14:50:08.000000 django-money-3.2.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-07-03 14:50:08.000000 django-money-3.2.0/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39496 2023-07-03 14:50:08.000000 django-money-3.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-03 14:50:08.000000 django-money-3.2.0/tests/test_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-03 14:50:08.000000 django-money-3.2.0/tests/test_reversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-03 14:50:08.000000 django-money-3.2.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-03 14:50:08.000000 django-money-3.2.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-03 14:50:08.000000 django-money-3.2.0/tests/test_tags.py
```

### Comparing `django-money-3.1.0/LICENSE.txt` & `django-money-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/PKG-INFO` & `django-money-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-money
-Version: 3.1.0
+Version: 3.2.0
 Summary: Adds support for using money and currency fields in django models and forms. Uses py-moneyed as the money implementation.
 Home-page: https://github.com/django-money/django-money
 Maintainer: Greg Reinbach
 Maintainer-email: greg@reinbach.com
 License: BSD
 Keywords: django,py-money,money
 Platform: Any
```

### Comparing `django-money-3.1.0/README.rst` & `django-money-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/django_money.egg-info/PKG-INFO` & `django-money-3.2.0/django_money.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-money
-Version: 3.1.0
+Version: 3.2.0
 Summary: Adds support for using money and currency fields in django models and forms. Uses py-moneyed as the money implementation.
 Home-page: https://github.com/django-money/django-money
 Maintainer: Greg Reinbach
 Maintainer-email: greg@reinbach.com
 License: BSD
 Keywords: django,py-money,money
 Platform: Any
```

### Comparing `django-money-3.1.0/django_money.egg-info/SOURCES.txt` & `django-money-3.2.0/django_money.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/_compat.py` & `django-money-3.2.0/djmoney/_compat.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/admin.py` & `django-money-3.2.0/djmoney/admin.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/contrib/django_rest_framework/fields.py` & `django-money-3.2.0/djmoney/contrib/django_rest_framework/fields.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/contrib/exchange/backends/base.py` & `django-money-3.2.0/djmoney/contrib/exchange/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/contrib/exchange/backends/fixer.py` & `django-money-3.2.0/djmoney/contrib/exchange/backends/fixer.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,8 +11,12 @@
     def __init__(self, url=settings.FIXER_URL, access_key=settings.FIXER_ACCESS_KEY):
         if access_key is None:
             raise ImproperlyConfigured("settings.FIXER_ACCESS_KEY should be set to use FixerBackend")
         self.url = url
         self.access_key = access_key
 
     def get_params(self):
-        return {"apikey": self.access_key}
+        # support both `data.fixer.io` and `api.apilayer.com` auth params
+        return {
+            "apikey": self.access_key,
+            "access_key": self.access_key,
+        }
```

### Comparing `django-money-3.1.0/djmoney/contrib/exchange/backends/openexchangerates.py` & `django-money-3.2.0/djmoney/contrib/exchange/backends/openexchangerates.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/contrib/exchange/management/base.py` & `django-money-3.2.0/djmoney/contrib/exchange/management/base.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/contrib/exchange/management/commands/clear_rates.py` & `django-money-3.2.0/djmoney/contrib/exchange/management/commands/clear_rates.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/contrib/exchange/migrations/0001_initial.py` & `django-money-3.2.0/djmoney/contrib/exchange/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/contrib/exchange/models.py` & `django-money-3.2.0/djmoney/contrib/exchange/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         return self.name
 
     def clear_rates(self):
         self.rates.all().delete()
 
 
 class Rate(models.Model):
+    id = models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")
     currency = models.CharField(max_length=CURRENCY_CODE_MAX_LENGTH)
     value = models.DecimalField(max_digits=20, decimal_places=6)
     backend = models.ForeignKey(ExchangeBackend, on_delete=models.CASCADE, related_name="rates")
 
     class Meta:
         unique_together = (("currency", "backend"),)
```

### Comparing `django-money-3.1.0/djmoney/forms/fields.py` & `django-money-3.2.0/djmoney/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/forms/widgets.py` & `django-money-3.2.0/djmoney/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/models/fields.py` & `django-money-3.2.0/djmoney/models/fields.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/models/managers.py` & `django-money-3.2.0/djmoney/models/managers.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/models/validators.py` & `django-money-3.2.0/djmoney/models/validators.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/money.py` & `django-money-3.2.0/djmoney/money.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/serializers.py` & `django-money-3.2.0/djmoney/serializers.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/settings.py` & `django-money-3.2.0/djmoney/settings.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/templatetags/djmoney.py` & `django-money-3.2.0/djmoney/templatetags/djmoney.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/djmoney/utils.py` & `django-money-3.2.0/djmoney/utils.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/setup.cfg` & `django-money-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/setup.py` & `django-money-3.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     long_description=read("README.rst"),
     long_description_content_type="text/x-rst",
     url="https://github.com/django-money/django-money",
     maintainer="Greg Reinbach",
     maintainer_email="greg@reinbach.com",
     license="BSD",
     packages=find_packages(include=["djmoney", "djmoney.*"]),
-    install_requires=["setuptools", "Django>=2.2", "py-moneyed>=2.0,<3.0"],
+    install_requires=["setuptools", "Django>=2.2", "py-moneyed>=2.0,<3.1"],
     python_requires=">=3.7",
     platforms=["Any"],
     keywords=["django", "py-money", "money"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
```

### Comparing `django-money-3.1.0/tests/test_admin.py` & `django-money-3.2.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/tests/test_form.py` & `django-money-3.2.0/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/tests/test_managers.py` & `django-money-3.2.0/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/tests/test_models.py` & `django-money-3.2.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/tests/test_money.py` & `django-money-3.2.0/tests/test_money.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/tests/test_reversion.py` & `django-money-3.2.0/tests/test_reversion.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/tests/test_serialization.py` & `django-money-3.2.0/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/tests/test_settings.py` & `django-money-3.2.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-money-3.1.0/tests/test_tags.py` & `django-money-3.2.0/tests/test_tags.py`

 * *Files identical despite different names*

