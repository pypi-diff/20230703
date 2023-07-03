# Comparing `tmp/django-pfx-1.2.dev84.tar.gz` & `tmp/django-pfx-1.2.dev86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pfx-1.2.dev84.tar", last modified: Mon Jul  3 09:13:38 2023, max compression
+gzip compressed data, was "django-pfx-1.2.dev86.tar", last modified: Mon Jul  3 09:45:15 2023, max compression
```

## Comparing `django-pfx-1.2.dev84.tar` & `django-pfx-1.2.dev86.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.533832 django-pfx-1.2.dev84/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-03 09:13:38.533832 django-pfx-1.2.dev84/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.517832 django-pfx-1.2.dev84/django_pfx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3417 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 09:13:38.000000 django-pfx-1.2.dev84/django_pfx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.518832 django-pfx-1.2.dev84/img/
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/img/pfx.png
--rw-rw-rw-   0 root         (0) root         (0)     2682 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/img/pfx.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.518832 django-pfx-1.2.dev84/pfx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.519832 django-pfx-1.2.dev84/pfx/pfxcore/
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.520832 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apidoc/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.520832 django-pfx-1.2.dev84/pfx/pfxcore/decorator/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/decorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/decorator/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.521832 django-pfx-1.2.dev84/pfx/pfxcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/http/json_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.513831 django-pfx-1.2.dev84/pfx/pfxcore/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.513831 django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.521832 django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     3331 2023-07-03 09:13:34.000000 django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     5332 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.521832 django-pfx-1.2.dev84/pfx/pfxcore/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.522832 django-pfx-1.2.dev84/pfx/pfxcore/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7568 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/management/commands/makeapidoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.522832 django-pfx-1.2.dev84/pfx/pfxcore/middleware/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/middleware/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/middleware/locale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.523832 django-pfx-1.2.dev84/pfx/pfxcore/models/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/cache_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/not_null_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3419 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/pfx_models.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/models/user_filtered_queryset_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.523832 django-pfx-1.2.dev84/pfx/pfxcore/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/serializers/json.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2936 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.524832 django-pfx-1.2.dev84/pfx/pfxcore/storage/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/storage/s3_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.514832 django-pfx-1.2.dev84/pfx/pfxcore/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.524832 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/welcome_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/templates/registration/welcome_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)    10198 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/test.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.525832 django-pfx-1.2.dev84/pfx/pfxcore/views/
--rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11581 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/authentication_views.py
--rw-rw-rw-   0 root         (0) root         (0)    12218 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4561 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/filters_views.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/locale_views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.528832 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/date_format.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_count.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_items.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_order.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_search.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/media_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/meta_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/meta_filters.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/meta_orders.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_limit.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_offset.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_page.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_page_size.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset_page_subset.py
--rw-rw-rw-   0 root         (0) root         (0)    27547 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pfx/pfxcore/views/rest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      440 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/runtest.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-03 09:13:38.534832 django-pfx-1.2.dev84/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.529832 django-pfx-1.2.dev84/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6487 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.530832 django-pfx-1.2.dev84/tests/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/dev.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/dev_custom_example.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/settings/dev_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:13:38.533832 django-pfx-1.2.dev84/tests/tests/
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/basic_api_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    46979 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/basic_api_test.py
--rw-rw-rw-   0 root         (0) root         (0)    18097 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_api_doc.py
--rw-rw-rw-   0 root         (0) root         (0)    29106 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     9909 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_locale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_perm_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     3725 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_perms_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_shortcuts.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_timezone_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_user_queryset.py
--rw-rw-rw-   0 root         (0) root         (0)     3558 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_view_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7356 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/tests/test_view_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8416 2023-07-03 09:12:55.000000 django-pfx-1.2.dev84/tests/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.662264 django-pfx-1.2.dev86/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-03 09:45:15.663264 django-pfx-1.2.dev86/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.645265 django-pfx-1.2.dev86/django_pfx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-03 09:45:15.000000 django-pfx-1.2.dev86/django_pfx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-07-03 09:45:15.000000 django-pfx-1.2.dev86/django_pfx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 09:45:15.000000 django-pfx-1.2.dev86/django_pfx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-03 09:45:15.000000 django-pfx-1.2.dev86/django_pfx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-03 09:45:15.000000 django-pfx-1.2.dev86/django_pfx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.645265 django-pfx-1.2.dev86/img/
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/img/pfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/img/pfx.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.645265 django-pfx-1.2.dev86/pfx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.647265 django-pfx-1.2.dev86/pfx/pfxcore/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.648265 django-pfx-1.2.dev86/pfx/pfxcore/apidoc/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/apidoc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/apidoc/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/apidoc/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/apidoc/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.648265 django-pfx-1.2.dev86/pfx/pfxcore/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/decorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2434 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/decorator/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.649265 django-pfx-1.2.dev86/pfx/pfxcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/http/json_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.640265 django-pfx-1.2.dev86/pfx/pfxcore/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.640265 django-pfx-1.2.dev86/pfx/pfxcore/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.649265 django-pfx-1.2.dev86/pfx/pfxcore/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-07-03 09:45:11.000000 django-pfx-1.2.dev86/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     5332 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.649265 django-pfx-1.2.dev86/pfx/pfxcore/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.650265 django-pfx-1.2.dev86/pfx/pfxcore/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7568 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/management/commands/makeapidoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.650265 django-pfx-1.2.dev86/pfx/pfxcore/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2706 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/middleware/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/middleware/locale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.651265 django-pfx-1.2.dev86/pfx/pfxcore/models/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/models/cache_mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/models/not_null_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3419 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/models/pfx_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/models/user_filtered_queryset_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.652264 django-pfx-1.2.dev86/pfx/pfxcore/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/serializers/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.652264 django-pfx-1.2.dev86/pfx/pfxcore/storage/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/storage/s3_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.641265 django-pfx-1.2.dev86/pfx/pfxcore/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.653265 django-pfx-1.2.dev86/pfx/pfxcore/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/templates/registration/welcome_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/templates/registration/welcome_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)    10198 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.654265 django-pfx-1.2.dev86/pfx/pfxcore/views/
+-rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11581 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/authentication_views.py
+-rw-rw-rw-   0 root         (0) root         (0)    12218 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/filters_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/locale_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.657265 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/date_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/list_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/list_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/list_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/list_order.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/list_search.py
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/media_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/meta_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/meta_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/meta_orders.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/subset.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/subset_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/subset_offset.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/subset_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/subset_page_size.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/subset_page_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)    28521 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pfx/pfxcore/views/rest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      440 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/runtest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-03 09:45:15.663264 django-pfx-1.2.dev86/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.658264 django-pfx-1.2.dev86/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6487 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.659264 django-pfx-1.2.dev86/tests/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/settings/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/settings/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/settings/dev_custom_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/settings/dev_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 09:45:15.662264 django-pfx-1.2.dev86/tests/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/basic_api_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    46979 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/basic_api_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    19335 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_api_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)    29106 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     9909 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_locale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_perm_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_perms_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_shortcuts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_timezone_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_user_queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3558 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_view_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/tests/test_view_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     8416 2023-07-03 09:44:33.000000 django-pfx-1.2.dev86/tests/views.py
```

### Comparing `django-pfx-1.2.dev84/.gitlab-ci.yml` & `django-pfx-1.2.dev86/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/LICENSE` & `django-pfx-1.2.dev86/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/PKG-INFO` & `django-pfx-1.2.dev86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev84
+Version: 1.2.dev86
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev84/README.md` & `django-pfx-1.2.dev86/README.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/django_pfx.egg-info/PKG-INFO` & `django-pfx-1.2.dev86/django_pfx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev84
+Version: 1.2.dev86
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev84/django_pfx.egg-info/SOURCES.txt` & `django-pfx-1.2.dev86/django_pfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/img/pfx.png` & `django-pfx-1.2.dev86/img/pfx.png`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/img/pfx.svg` & `django-pfx-1.2.dev86/img/pfx.svg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/apidoc/parameters.py` & `django-pfx-1.2.dev86/pfx/pfxcore/apidoc/parameters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/apidoc/schema.py` & `django-pfx-1.2.dev86/pfx/pfxcore/apidoc/schema.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/decorator/rest.py` & `django-pfx-1.2.dev86/pfx/pfxcore/decorator/rest.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from pfx.pfxcore.exceptions import APIError
 from pfx.pfxcore.http import JsonResponse
 
 logger = logging.getLogger(__name__)
 
 
 def rest_api(
-        path, method='get', public=None, priority=0, parameters=None,
+        path, method='get', public=None, priority=0, priority_doc=100,
+        parameters=None,
         request_schema=None, response_schema=None, filters=False,
         groups=None):
     def decorator(func):
         @wraps(func)
         def wrapper(self, request, *args, **kwargs):
             self.request = request
             self.kwargs = kwargs
@@ -32,14 +33,15 @@
             except Exception as e:
                 logger.exception(e)
                 return JsonResponse(dict(message=_(
                     "An internal server error occured.")), status=500)
         wrapper.rest_api_path = path
         wrapper.rest_api_method = method
         wrapper.rest_api_priority = priority
+        wrapper.rest_api_priority_doc = priority_doc
         wrapper.rest_api_params = parameters or []
         wrapper.rest_api_request_schema = request_schema
         wrapper.rest_api_response_schema = response_schema
         wrapper.rest_api_filters = filters
         wrapper.rest_api_groups = set(groups or [])
         wrapper.rest_api_public = public
         return wrapper
```

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/exceptions.py` & `django-pfx-1.2.dev86/pfx/pfxcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/fields.py` & `django-pfx-1.2.dev86/pfx/pfxcore/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo` & `django-pfx-1.2.dev86/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po` & `django-pfx-1.2.dev86/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/management/commands/makeapidoc.py` & `django-pfx-1.2.dev86/pfx/pfxcore/management/commands/makeapidoc.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/middleware/authentication.py` & `django-pfx-1.2.dev86/pfx/pfxcore/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/middleware/locale.py` & `django-pfx-1.2.dev86/pfx/pfxcore/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/models/cache_mixins.py` & `django-pfx-1.2.dev86/pfx/pfxcore/models/cache_mixins.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/models/pfx_models.py` & `django-pfx-1.2.dev86/pfx/pfxcore/models/pfx_models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/shortcuts.py` & `django-pfx-1.2.dev86/pfx/pfxcore/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/storage/s3_storage.py` & `django-pfx-1.2.dev86/pfx/pfxcore/storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/test.py` & `django-pfx-1.2.dev86/pfx/pfxcore/test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/__init__.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/authentication_views.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/authentication_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/fields.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/filters_views.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/filters_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/locale_views.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/locale_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/__init__.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/date_format.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/date_format.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/groups.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/groups.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/list_order.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/list_order.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/parameters/subset.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/parameters/subset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/pfx/pfxcore/views/rest_views.py` & `django-pfx-1.2.dev86/pfx/pfxcore/views/rest_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,15 +198,16 @@
         meta = {}
         defaults = {} if self.request.GET.keys() else dict(fields=True)
         if get_bool(self.request.GET, 'fields', defaults.get('fields')):
             meta['fields'] = {
                 n: f.meta() for n, f in self.get_fields().items()}
         return meta
 
-    @rest_api("/meta", method="get", response_schema='meta_schema')
+    @rest_api(
+        "/meta", method="get", response_schema='meta_schema', priority_doc=20)
     def get_meta(self, *args, **kwargs):
         """Retrieve the model metadata.
         ---
         get:
             summary: Get {model} metadata
         """
         return JsonResponse(self.object_meta())
@@ -325,15 +326,16 @@
         if get_bool(self.request.GET, 'filters', default_all):
             meta['filters'] = [f.meta for f in self.filters]
         if get_bool(self.request.GET, 'orders', default_all):
             meta['orders'] = list(self.orderable_fields(self.model))
         return meta
 
     @rest_api("/meta/list", method="get", parameters=[
-        parameters.groups.MetaList], response_schema='meta_list_schema')
+        parameters.groups.MetaList], response_schema='meta_list_schema',
+        priority_doc=10)
     def get_meta_list(self, *args, **kwargs):
         """Retrieve the model list metadata.
         ---
         get:
             summary: Get {models} list metadata
         """
         return JsonResponse(self.object_meta_list())
@@ -403,15 +405,15 @@
             count=count,
             page_count=page_count,
             limit=limit,
             offset=offset)
 
     @rest_api(
         "", method="get", parameters=[parameters.groups.List], filters=True,
-        response_schema='model_list_schema')
+        response_schema='model_list_schema', priority_doc=-20)
     def get_list(self, *args, **kwargs):
         """Retrieve a list of model.
         ---
         get:
             summary: Get {models} list
         """
         res = {}
@@ -489,15 +491,16 @@
     def get_apidoc_schemas(cls):
         return super().get_apidoc_schemas() + [
             cls.meta_list_schema, cls.model_list_schema]
 
 
 class DetailRestViewMixin(ModelResponseMixin):
     @rest_api("/<int:id>", method="get", parameters=[
-        parameters.groups.ModelSerialization], response_schema='model_schema')
+        parameters.groups.ModelSerialization], response_schema='model_schema',
+        priority_doc=-10)
     def get(self, id, *args, **kwargs):
         """Retrieve the model by pk.
         ---
         get:
             summary: Get {model}
             parameters extras:
                 id: the {model} pk
@@ -505,16 +508,18 @@
         obj = self.get_object(pk=id)
         return self.response(obj)
 
 
 class SlugDetailRestViewMixin(ModelResponseMixin):
     SLUG_FIELD = "slug"
 
-    @rest_api("/slug/<slug:slug>", method="get", parameters=[
-        parameters.groups.ModelSerialization], response_schema='model_schema')
+    @rest_api(
+        "/slug/<slug:slug>", method="get",
+        parameters=[parameters.groups.ModelSerialization],
+        response_schema='model_schema', priority_doc=-10)
     def get_by_slug(self, slug, *args, **kwargs):
         """Retrieve the model by slug.
         ---
         get:
             summary: Get {model} by slug
             parameters extras:
                 slug: the {model} slug name
@@ -550,15 +555,15 @@
             return self.is_valid(obj, created=True, rel_data=rel_data)
         except ValidationError as e:
             return self.is_invalid(obj, errors=e)
 
     @rest_api(
         "", method="post", parameters=[parameters.groups.ModelSerialization],
         request_schema='model_create_schema',
-        response_schema='model_message_schema')
+        response_schema='model_message_schema', priority_doc=-20)
     def post(self, *args, **kwargs):
         """Create the model.
         ---
         post:
             summary: Create {model}
         """
         return self._post(*args, **kwargs)
@@ -584,15 +589,16 @@
         except ValidationError as e:
             return self.is_invalid(obj, errors=e)
 
     @rest_api(
         "/<int:id>", method="put",
         parameters=[parameters.groups.ModelSerialization],
         request_schema='model_update_schema',
-        response_schema='model_message_schema')
+        response_schema='model_message_schema',
+        priority_doc=-10)
     def put(self, id, *args, **kwargs):
         """Update the model by pk.
         ---
         put:
             summary: Update {model}
             parameters extras:
                 id: the {model} pk
@@ -608,15 +614,17 @@
         obj = self.get_object(pk=id)
         if not self.object_delete_perm(obj):
             raise ForbiddenError()
         self.delete_object(obj)
         return self.message_response(f(
             _("{model} {obj} deleted."), model=self.model_name, obj=obj))
 
-    @rest_api("/<int:id>", method="delete", response_schema='message_schema')
+    @rest_api(
+        "/<int:id>", method="delete", response_schema='message_schema',
+        priority_doc=-10)
     def delete(self, id, *args, **kwargs):
         """Delete the model by pk.
         ---
         delete:
             summary: Delete {model}
             parameters extras:
                 id: the {model} pk
@@ -630,15 +638,17 @@
             model_field = self.model._meta.get_field(field)
             if not isinstance(model_field, MediaField):
                 raise NotFoundError  # pragma: no cover
         except FieldDoesNotExist:  # pragma: no cover
             raise NotFoundError
         return model_field
 
-    @rest_api("/<int:pk>/<str:field>/upload-url/<str:filename>", method="get")
+    @rest_api(
+        "/<int:pk>/<str:field>/upload-url/<str:filename>", method="get",
+        priority_doc=-8)
     def field_media_upload_url(self, pk, field, filename, *args, **kwargs):
         """Get upload URL for a media field.
         ---
         get:
             summary: Get upload URL
             description: Get upload URL for a file field.
             parameters extras:
@@ -651,16 +661,17 @@
             res = self._get_model_field(field).get_upload_url(
                 self.request, obj, filename)
         except StorageException as e:  # pragma: no cover
             logger.exception(e)
             raise APIError(_("Unexpected storage error", status=500))
         return JsonResponse(res)
 
-    @rest_api("/<int:pk>/<str:field>", method="get", parameters=[
-        parameters.MediaRedirect])
+    @rest_api(
+        "/<int:pk>/<str:field>", method="get",
+        parameters=[parameters.MediaRedirect], priority_doc=-9)
     def field_media_get(self, pk, field, *args, **kwargs):
         """Get the URL for a media field file.
         ---
         get:
             summary: Get {model} file
             description: Get the URL for a media field file.
             parameters extras:
@@ -734,40 +745,55 @@
             e = re.sub(r'<str:.*>', '!06', e)
             e = re.sub(r'<.*>', '!02', e)
             return e
 
         return methods.get('priority', 0), *map(
             process, path.lstrip('/').split('/'))
 
+    @staticmethod
+    def _path_order_doc(path, methods):
+        return methods.get('priority_doc', 0), path.lstrip('/').split('/')
+
     @classmethod
     def get_urls(cls, as_pattern=False):
         def fullpath(p2):
             res = f'{cls.rest_view_path[cls]}{p2}'.lstrip('/')
             return res if as_pattern else f'/{res}'
 
         paths = {}
         for name in dir(cls):
             m = getattr(cls, name, None)
             if m and callable(m) and hasattr(m, 'rest_api_method'):
-                methods = paths.setdefault(m.rest_api_path, dict(priority=0))
+                methods = paths.setdefault(m.rest_api_path, dict(
+                    priority=0, priority_doc=0))
                 methods[m.rest_api_method] = name
                 if m.rest_api_priority != 0:
                     if methods['priority'] not in (0, m.rest_api_priority):
                         raise Exception(
                             f"Path {fullpath(m.rest_api_path)}: "
                             "you cannot set different priority for same path")
                     methods['priority'] = m.rest_api_priority
+                if m.rest_api_priority_doc != 0:
+                    if methods['priority_doc'] not in (
+                            0, m.rest_api_priority_doc):
+                        raise Exception(
+                            f"Path {fullpath(m.rest_api_path)}: "
+                            "you cannot set different priority_doc "
+                            "for same path")
+                    methods['priority_doc'] = m.rest_api_priority_doc
         return [
             path(fullpath(p), cls.as_view(pfx_methods=ms)) if as_pattern
             else dict(path=fullpath(p), methods={
-                k: v for k, v in ms.items() if k != 'priority'})
+                k: v for k, v in ms.items()
+                if k not in ('priority', 'priority_doc')})
             for p, ms in sorted(
                 paths.items(), key=lambda e:
-                    cls._path_order(*e) if as_pattern else e[0],
-                reverse=True)]
+                    cls._path_order(*e) if as_pattern
+                    else cls._path_order_doc(*e),
+                reverse=as_pattern)]
 
     @classmethod
     def as_urlpatterns(cls):
         if cls not in __PFX_VIEWS__:
             __PFX_VIEWS__.append(cls)
         return cls.get_urls(as_pattern=True)
```

### Comparing `django-pfx-1.2.dev84/setup.cfg` & `django-pfx-1.2.dev86/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/models.py` & `django-pfx-1.2.dev86/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/settings/common.py` & `django-pfx-1.2.dev86/tests/settings/common.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/settings/dev_custom_example.py` & `django-pfx-1.2.dev86/tests/settings/dev_custom_example.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/__init__.py` & `django-pfx-1.2.dev86/tests/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/basic_api_errors.py` & `django-pfx-1.2.dev86/tests/tests/basic_api_errors.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/basic_api_test.py` & `django-pfx-1.2.dev86/tests/tests/basic_api_test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_api_doc.py` & `django-pfx-1.2.dev86/tests/tests/test_api_doc.py`

 * *Files 9% similar despite different names*

```diff
@@ -293,14 +293,45 @@
         self.assertJENotExists(props, 'created_at')
         # Check foreign object can be number/object
         self.assertJE(props, 'author.oneOf.@0.type', 'number')
         self.assertJE(props, 'author.oneOf.@1.type', 'object')
         self.assertSize(props, 'author.oneOf.@1.properties', 1)
         self.assertJE(props, 'author.oneOf.@1.properties.pk.type', 'number')
 
+    def test_paths_order(self):
+        spec = get_spec(set()).to_dict()
+        paths = self.get_val(spec, 'paths')
+        authors_paths = [p for p in paths if p.startswith('/authors')]
+        self.assertEqual(authors_paths[:11], [
+            '/authors',
+            '/authors/{pk}',
+            '/authors/slug/{slug}',
+            '/authors/meta/list',
+            '/authors/meta',
+            '/authors/cache/{pk}',
+            '/authors/priority/{value}',
+            '/authors/priority/default',
+            '/authors/priority/default/path',
+            '/authors/priority/priority-less',
+            '/authors/priority/priority-more'])
+        books_paths = [p for p in paths if p.startswith('/books')]
+        self.assertEqual(books_paths, [
+            "/books",
+            "/books/{pk}",
+            "/books/{pk}/{field}",
+            "/books/{pk}/{field}/upload-url/{filename}",
+            "/books/meta/list",
+            "/books/meta",
+            "/books-custom-author",
+            "/books-custom-author/{pk}",
+            "/books-custom-author/{pk}/{field}",
+            "/books-custom-author/{pk}/{field}/upload-url/{filename}",
+            "/books-custom-author/meta/list",
+            "/books-custom-author/meta"])
+
     def test_groups(self):
         spec = get_spec(set()).to_dict()
         self.assertJEExists(spec, 'paths./authors/cache/{pk}.get')
         self.assertJEExists(spec, 'paths./authors-annotate/{pk}.get')
 
         spec = get_spec({'cache', }).to_dict()
         self.assertJEExists(spec, 'paths./authors/cache/{pk}.get')
```

### Comparing `django-pfx-1.2.dev84/tests/tests/test_auth_api.py` & `django-pfx-1.2.dev86/tests/tests/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_cache.py` & `django-pfx-1.2.dev86/tests/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_fields.py` & `django-pfx-1.2.dev86/tests/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_filters.py` & `django-pfx-1.2.dev86/tests/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_locale_api.py` & `django-pfx-1.2.dev86/tests/tests/test_locale_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_perm_tests.py` & `django-pfx-1.2.dev86/tests/tests/test_perm_tests.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_perms_api.py` & `django-pfx-1.2.dev86/tests/tests/test_perms_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_shortcuts.py` & `django-pfx-1.2.dev86/tests/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_timezone_middleware.py` & `django-pfx-1.2.dev86/tests/tests/test_timezone_middleware.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_tools.py` & `django-pfx-1.2.dev86/tests/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_user_queryset.py` & `django-pfx-1.2.dev86/tests/tests/test_user_queryset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_view_decorators.py` & `django-pfx-1.2.dev86/tests/tests/test_view_decorators.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/tests/test_view_fields.py` & `django-pfx-1.2.dev86/tests/tests/test_view_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/urls.py` & `django-pfx-1.2.dev86/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev84/tests/views.py` & `django-pfx-1.2.dev86/tests/views.py`

 * *Files identical despite different names*

